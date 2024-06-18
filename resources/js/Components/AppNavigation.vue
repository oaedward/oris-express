<script setup lang="ts">
import { Menu } from "lucide-vue-next";
import { Link } from "@inertiajs/vue3";
import { Button } from "@/Components/ui/button";

import {
    NavigationMenu,
    NavigationMenuContent,
    NavigationMenuItem,
    NavigationMenuList,
    NavigationMenuTrigger,
    navigationMenuTriggerStyle,
    NavigationList,
} from "@/Components/ui/navigation-menu";

import {
    Sheet,
    SheetContent,
    SheetDescription,
    SheetHeader,
    SheetTitle,
    SheetTrigger,
} from "@/Components/ui/sheet";

import {
    Accordion,
    AccordionContent,
    AccordionItem,
    AccordionTrigger,
} from "@/Components/ui/accordion";

const components: { title: string; href: string }[] = [
    {
        title: "Education",
        href: "services",
    },
    {
        title: "Business Development",
        href: "services",
    },
    {
        title: "Biomedical",
        href: "services",
    },
    {
        title: "Handyman",
        href: "services",
    },
];
</script>

<template>
    <div class="">
        <NavigationMenu class="hidden lg:block">
            <NavigationMenuList>
                <NavigationMenuItem>
                    <Link
                        :href="route('home')"
                        :class="navigationMenuTriggerStyle()"
                        >Home</Link
                    >
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <Link
                        :href="route('home')"
                        :class="navigationMenuTriggerStyle()"
                        >About</Link
                    >
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <NavigationMenuTrigger>Services</NavigationMenuTrigger>
                    <NavigationMenuContent>
                        <ul
                            class="grid w-[48px] gap-3 p-2 md:w-[48px] md:grid-cols-1 lg:w-[200px]"
                        >
                            <NavigationList
                                v-for="component in components"
                                :key="component.title"
                                :title="component.title"
                                :href="route(component.href)"
                                class=""
                            />
                        </ul>
                    </NavigationMenuContent>
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <Link
                        :href="route('home')"
                        :class="navigationMenuTriggerStyle()"
                        >Contact</Link
                    >
                </NavigationMenuItem>
            </NavigationMenuList>
        </NavigationMenu>

        <Sheet>
            <SheetTrigger class="block lg:hidden">
                <Button variant="outline">
                    <Menu class="w-4 h-4" />
                </Button>
            </SheetTrigger>
            <SheetContent side="left" class="w-[350px]">
                <SheetHeader>
                    <SheetTitle>
                        <h2 class="mb-2 px-4 text-lg font-semibold text-left">
                            Oris Express
                        </h2>
                    </SheetTitle>
                </SheetHeader>
                <SheetDescription>
                    <div class="flex flex-col gap-1">
                        <div class="border-b py-2">
                            <Link :href="route('home')">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    Home
                                </Button>
                            </Link>
                        </div>
                        <div class="border-b py-2">
                            <Link :href="route('home')">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    About
                                </Button>
                            </Link>
                        </div>
                        <div class="">
                            <Accordion
                                type="single"
                                collapsible
                                class="w-full justify-start"
                            >
                                <AccordionItem value="item-1">
                                    <AccordionTrigger class="px-4"
                                        >Services</AccordionTrigger
                                    >
                                    <AccordionContent>
                                        <div
                                            class="flex flex-col gap-1 px-4 py-1"
                                            v-for="component in components"
                                            :key="component.title"
                                        >
                                            <Link :href="component.href">
                                                <Button
                                                    variant="ghost"
                                                    class="w-full justify-start"
                                                >
                                                    {{ component.title }}
                                                </Button>
                                            </Link>
                                        </div>
                                    </AccordionContent>
                                </AccordionItem>
                            </Accordion>
                        </div>

                        <div class="border-b py-2">
                            <Link :href="route('home')">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    Contact
                                </Button>
                            </Link>
                        </div>
                    </div>
                </SheetDescription>
            </SheetContent>
        </Sheet>
    </div>
</template>

<style scoped></style>
