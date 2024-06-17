<template>
    <section class="bg-primary">
        <div class="container flex flex-col justify-between py-6 sm:flex-row">
            <p class="text-center font-body text-white md:text-left">
                &copy; {{ date }} Oris Express. All rights reserved
            </p>
            <div
                class="flex items-center justify-center pt-5 sm:justify-start sm:pt-0"
            >
                <a href="/">
                    <i
                        class="bx bxl-facebook-square text-2xl text-white hover:text-yellow"
                    ></i>
                </a>
                <a href="/" class="pl-4">
                    <i
                        class="bx bxl-twitter text-2xl text-white hover:text-yellow"
                    ></i>
                </a>
                <a href="/" class="pl-4">
                    <i
                        class="bx bxl-dribbble text-2xl text-white hover:text-yellow"
                    ></i>
                </a>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { ref } from "vue";

const date = ref(new Date().getFullYear());
</script>

<style scoped></style>
