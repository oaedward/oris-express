<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
import ApplicationLogo from "@/Components/ApplicationLogo.vue";
import AppFooter from "@/Components/AppFooter.vue";
import AppNavigation from "@/Components/AppNavigation.vue";
</script>

<template>
    <div class="flex-col md:flex scroll-smooth">
        <header class="border-b border-b-accent bg-background p-2">
            <div class="container flex items-center justify-between">
                <div class="font-bold">
                    <Link :href="route('home')">
                        <ApplicationLogo
                            class="block h-9 w-auto fill-current text-gray-800 dark:text-gray-200"
                        />
                    </Link>
                </div>
                <div class="">
                    <AppNavigation />
                </div>
            </div>
        </header>
        <main class="bg-background">
            <div>
                <slot />
            </div>
        </main>
        <footer>
            <AppFooter />
        </footer>
    </div>
</template>

<style scoped></style>
