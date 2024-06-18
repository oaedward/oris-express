<template>
    <section class="flex items-center min-h-screen justify-center bg-white">
        <div class="mx-auto max-w-[43rem]">
            <div class="text-center">
                <p class="text-lg font-medium leading-8 text-primary">
                    Introducing the Oris Express Platform
                </p>
                <h1
                    class="mt-3 text-[3.5rem] font-bold leading-[4rem] tracking-tight text-black"
                >
                    Welcome to Oris Express
                </h1>
                <p class="mt-3 text-md leading-relaxed text-slate-400">
                    Explore all our services and products to find your right
                    solution.
                </p>
            </div>

            <div class="mt-6 flex items-center justify-center gap-4">
                <a
                    href="#about"
                    v-smooth-scroll
                    class="transform rounded-md text-white transition-colors transition-al l duration-300"
                    ><Button variant="secondary">
                        <MoveDown
                            :size="28"
                            class="animate-bounce text-primary"
                        /> </Button
                ></a>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { Button } from "@/Components/ui/button";
import { MoveDown } from "lucide-vue-next";
</script>

<style scoped></style>
