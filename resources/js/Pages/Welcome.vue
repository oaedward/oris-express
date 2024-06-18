<script setup lang="ts">
import { Head } from "@inertiajs/vue3";
import MainLayout from "@/Layouts/MainLayout.vue";
import HeroSection from "@/Components/HeroSection.vue";
import AboutSection from "@/Components/AboutSection.vue";
import CoreValuesSection from "@/Components/CoreValuesSection.vue";
import ServiceSection from "@/Components/ServiceSection.vue";
</script>

<template>
    <MainLayout>
        <Head title="Oris Express" />
        <div class="dark:bg-gray-900 dark:text-white/50">
            <HeroSection id="hero" />
            <AboutSection id="about" />
            <CoreValuesSection />
            <ServiceSection id="services" />
            <ContactSetion id="contact" />
        </div>
    </MainLayout>
</template>
