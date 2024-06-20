<template>
    <MainLayout>
        <Head title="Oris Express" />
        <PageHeader title="About Us" />
        <div>
            <AboutSection id="about" />
            <MissionViosionSection />
            <CoreValuesSection />
            <TeamsSection />
        </div>
    </MainLayout>
</template>

<script setup lang="ts">
import { Head } from "@inertiajs/vue3";
import MainLayout from "@/Layouts/MainLayout.vue";
import PageHeader from "@/Components/PageHeader.vue";
import AboutSection from "@/Components/AboutSection.vue";
import MissionViosionSection from "@/Components/MissionViosionSection.vue";
import CoreValuesSection from "@/Components/CoreValuesSection.vue";
import TeamsSection from "@/Components/TeamsSection.vue";
</script>

<style scoped></style>
