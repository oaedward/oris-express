<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
import ApplicationLogo from "@/Components/ApplicationLogo.vue";
import AppFooter from "@/Components/AppFooter.vue";
</script>

<template>
    <div class="flex-col md:flex scroll-smooth">
        <div
            class="sticky top-0 z-20 border-b border-b-accent bg-background p-2"
        >
            <div class="container flex items-center justify-between">
                <div class="font-bold">
                    <Link :href="route('dashboard')">
                        <ApplicationLogo
                            class="block h-9 w-auto fill-current text-gray-800 dark:text-gray-200"
                        />
                    </Link>
                </div>
                <div class="">
                    <!-- <MainNav class="" /> -->
                </div>
            </div>
        </div>
        <div class="bg-background">
            <div class="">
                <slot />
            </div>
        </div>
        <div>
            <AppFooter />
        </div>
    </div>
</template>

<style scoped></style>
