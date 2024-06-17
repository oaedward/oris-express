<script setup lang="ts">
import { RouterLink } from "vue-router";
import { Menu } from "lucide-vue-next";
import { Button } from "../ui/button";

import {
    NavigationMenu,
    NavigationMenuContent,
    NavigationMenuItem,
    NavigationMenuLink,
    NavigationMenuList,
    NavigationMenuTrigger,
    navigationMenuTriggerStyle,
    NavigationList,
} from "@/components/ui/navigation-menu";

import {
    Sheet,
    SheetContent,
    SheetDescription,
    SheetHeader,
    SheetTitle,
    SheetTrigger,
} from "@/components/ui/sheet";

import {
    Accordion,
    AccordionContent,
    AccordionItem,
    AccordionTrigger,
} from "@/components/ui/accordion";

// const side = 'left' as const

const components: { title: string; href: string; description: string }[] = [
    {
        title: "Education",
        href: "/education",
        description: "Education Services",
    },
    {
        title: "Biomedical",
        href: "/services",
        description: "Biomedical Services",
    },
    {
        title: "Handyman",
        href: "/services",
        description: "Handyman Services",
    },
];
</script>

<template>
    <div class="">
        <NavigationMenu class="hidden lg:block">
            <NavigationMenuList>
                <NavigationMenuItem>
                    <NavigationMenuLink
                        href="/"
                        :class="navigationMenuTriggerStyle()"
                    >
                        Home
                    </NavigationMenuLink>
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <NavigationMenuLink
                        href="/about"
                        :class="navigationMenuTriggerStyle()"
                    >
                        About
                    </NavigationMenuLink>
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <NavigationMenuTrigger>Services</NavigationMenuTrigger>
                    <NavigationMenuContent>
                        <ul
                            class="grid w-[400px] gap-3 p-4 md:w-[300px] md:grid-cols-1 lg:w-[400px]"
                        >
                            <NavigationList
                                v-for="component in components"
                                :key="component.title"
                                :title="component.title"
                                :href="component.href"
                                class=""
                            >
                                {{ component.description }}
                            </NavigationList>
                        </ul>
                    </NavigationMenuContent>
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <NavigationMenuLink
                        href="/contact"
                        :class="navigationMenuTriggerStyle()"
                    >
                        Contact
                    </NavigationMenuLink>
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
                            <router-link to="/">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    Home
                                </Button>
                            </router-link>
                        </div>
                        <div class="border-b py-2">
                            <router-link to="/about">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    About
                                </Button>
                            </router-link>
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
                                            :key="component.description"
                                        >
                                            <router-link :to="component.href">
                                                <Button
                                                    variant="ghost"
                                                    class="w-full justify-start"
                                                >
                                                    {{ component.title }}
                                                </Button>
                                            </router-link>
                                        </div>
                                    </AccordionContent>
                                </AccordionItem>
                            </Accordion>
                        </div>

                        <div class="border-b py-2">
                            <router-link to="/contact">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    Contact
                                </Button>
                            </router-link>
                        </div>
                    </div>
                </SheetDescription>
            </SheetContent>
        </Sheet>
    </div>
</template>

<style scoped></style>
