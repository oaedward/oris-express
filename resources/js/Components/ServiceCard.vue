<template>
    <div class="group rounded px-2 py-12 shadow hover:bg-primary">
        <div class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28">
            <div class="hidden group-hover:block">
                <img :src="image" :alt="alt" />
            </div>
            <div class="block group-hover:hidden">
                <img
                    src="/assets/img/icon-development-black.svg"
                    alt="development icon"
                />
            </div>
        </div>
        <div class="text-center">
            <h3
                class="pt-8 text-lg font-semibold text-primary group-hover:text-accent lg:text-xl"
            >
                {{ title }}
            </h3>
            <p
                class="text-gray-600 pt-4 text-sm group-hover:text-white md:text-base"
            >
                {{ description }}
            </p>
        </div>
    </div>
</template>

<script setup lang="ts">
defineProps<{
    title: string;
    description: string;
    image: string;
    alt: string;
}>();
</script>

<style scoped></style>
