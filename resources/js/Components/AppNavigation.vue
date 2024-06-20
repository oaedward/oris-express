<script setup lang="ts">
import { Menu } from "lucide-vue-next";
import { Link } from "@inertiajs/vue3";
import { Button } from "@/Components/ui/button";

import {
    NavigationMenu,
    NavigationMenuItem,
    NavigationMenuList,
    navigationMenuTriggerStyle,
} from "@/Components/ui/navigation-menu";

import {
    Sheet,
    SheetContent,
    SheetDescription,
    SheetHeader,
    SheetTitle,
    SheetTrigger,
} from "@/Components/ui/sheet";
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
                        :href="route('about')"
                        :class="navigationMenuTriggerStyle()"
                        >About</Link
                    >
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <Link
                        :href="route('services')"
                        :class="navigationMenuTriggerStyle()"
                        >Departments</Link
                    >
                </NavigationMenuItem>
                <NavigationMenuItem>
                    <Link
                        :href="route('contact')"
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
                            <Link :href="route('about')">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    About
                                </Button>
                            </Link>
                        </div>
                        <div class="border-b py-2">
                            <Link :href="route('services')">
                                <Button
                                    variant="ghost"
                                    class="w-full justify-start"
                                >
                                    Departments
                                </Button>
                            </Link>
                        </div>
                        <div class="border-b py-2">
                            <Link :href="route('contact')">
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
