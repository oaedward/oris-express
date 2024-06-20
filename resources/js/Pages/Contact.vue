<template>
    <MainLayout>
        <Head title="Oris Express - Contact" />
        <PageHeader title="Contact Us" />
        <div>
            <ContactSection />
        </div>
    </MainLayout>
</template>

<script setup lang="ts">
import { Head } from "@inertiajs/vue3";
import MainLayout from "@/Layouts/MainLayout.vue";
import PageHeader from "@/Components/PageHeader.vue";
import ContactSection from "@/Components/ContactSection.vue";
</script>

<style scoped></style>
