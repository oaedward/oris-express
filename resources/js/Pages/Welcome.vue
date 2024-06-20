<script setup lang="ts">
import { Head } from "@inertiajs/vue3";
import MainLayout from "@/Layouts/MainLayout.vue";
import HeroSection from "@/Components/HeroSection.vue";
import DepartmentSection from "@/Components/DepartmentSection.vue";
import AboutSummary from "@/Components/AboutSummary.vue";
import ServiceSection from "@/Components/ServiceSection.vue";
import WhyChooseUs from "@/Components/WhyChooseUs.vue";
import ContactSection from "@/Components/ContactSection.vue";
</script>

<template>
    <MainLayout>
        <Head title="Oris Express" />
        <div class="dark:bg-gray-900 dark:text-white/50">
            <HeroSection id="hero" />
            <AboutSummary id="about" />
            <DepartmentSection id="department" />
            <ServiceSection id="services" />
            <WhyChooseUs />
            <ContactSection id="contact" />
        </div>
    </MainLayout>
</template>
