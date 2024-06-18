<template>
    <section class="container py-16 md:py-20">
        <SectionHeader
            title="Our Services"
            subTitle="Explore the comprehensive services Oris Express has to offer"
        />

        <div
            class="grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:grid-cols-3 md:gap-2 md:pt-12 lg:grid-cols-4"
        >
            <ServiceCard
                title="Oris Education"
                description="New Description"
                image="sds"
                alt="Oris Education Image"
            />
            <ServiceCard
                title="Oris Business Development"
                description="New Description"
                image="sds"
                alt="Oris Education Image"
            />
            <ServiceCard
                title="Oris Biomedical"
                description="New Description"
                image="sds"
                alt="Oris Education Image"
            />
            <ServiceCard
                title="Oris Handyman"
                description="New Description"
                image="sds"
                alt="Oris Education Image"
            />
        </div>
    </section>
</template>

<script setup lang="ts">
import SectionHeader from "@/Components/SectionHeader.vue";
import ServiceCard from "@/Components/ServiceCard.vue";
</script>

<style scoped></style>
