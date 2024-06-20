<template>
    <nav class="bg-white shadow dark:bg-gray-800 sticky top-0 z-20">
        <div
            class="container flex items-center justify-between p-2 mx-auto text-gray-600 capitalize dark:text-gray-300"
        >
            <div>
                <Link :href="route('services')" class="flex gap-2 items-center">
                    <ApplicationLogo
                        class="block h-9 w-auto fill-current text-gray-800 dark:text-gray-200"
                    />
                    <span class="font-bold">{{ name }}</span>
                </Link>
            </div>
            <NavigationMenu class="lg:block">
                <NavigationMenuList>
                    <NavigationMenuItem>
                        <Link
                            :href="route('services')"
                            :class="navigationMenuTriggerStyle()"
                            >Overview</Link
                        >
                    </NavigationMenuItem>
                    <NavigationMenuItem>
                        <Link
                            :href="route('consult')"
                            :class="navigationMenuTriggerStyle()"
                            >Oris Consult</Link
                        >
                    </NavigationMenuItem>
                    <NavigationMenuItem>
                        <Link
                            :href="route('engineering')"
                            :class="navigationMenuTriggerStyle()"
                            >Oris Engieering</Link
                        >
                    </NavigationMenuItem>
                </NavigationMenuList>
            </NavigationMenu>
        </div>
    </nav>
</template>

<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
import ApplicationLogo from "@/Components/ApplicationLogo.vue";

import {
    NavigationMenu,
    NavigationMenuItem,
    NavigationMenuList,
    navigationMenuTriggerStyle,
} from "@/Components/ui/navigation-menu";

defineProps<{
    name?: string;
}>();
</script>

<style scoped></style>
