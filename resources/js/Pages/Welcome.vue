<script setup lang="ts">
import { Head, Link } from "@inertiajs/vue3";
import { Button } from "@/Components/ui/button";
import { MoveDown } from "lucide-vue-next";
</script>

<template>
    <MainLayout>
        <Head title="Oris Express" />
        <div class="bg-gray-100 dark:bg-gray-900 dark:text-white/50">
            <section
                class="py-24 flex items-center min-h-screen justify-center bg-white"
            >
                <div class="mx-auto max-w-[43rem]">
                    <div class="text-center">
                        <p class="text-lg font-medium leading-8 text-primary">
                            Introducing the Oris Express Platform
                        </p>
                        <h1
                            class="mt-3 text-[3.5rem] font-bold leading-[4rem] tracking-tight text-black"
                        >
                            Collaborate with Oris Express
                        </h1>
                        <p class="mt-3 text-md leading-relaxed text-slate-400">
                            Explore all our services and products to find your
                            right solution.
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
            <section class="bg-gray-100" id="about">
                <div
                    class="container flex flex-col items-center py-16 md:py-20 lg:flex-row"
                >
                    <div
                        class="w-full text-center sm:w-3/4 lg:w-3/5 lg:text-left"
                    >
                        <h2
                            class="text-[3.0rem] font-bold leading-[4rem] tracking-tight text-black sm:text-[3.5rem] lg:text-[3.5rem]"
                        >
                            Who we are?
                        </h2>
                        <h4
                            class="pt-3 text-md leading-relaxed text-black sm:text-2xl lg:text-md"
                        >
                            A comprehensive solutions expert
                        </h4>
                        <p class="pt-6 font-body leading-relaxed text-gray-20">
                            Lorem ipsum dolor sit amet, consectetur adipisicing
                            elit, sed do eiusmod tempor incididunt ut labore et
                            dolore magna aliqua. Ut enim ad minim veniam, quis
                            nostrud exercitation ullamco laboris nisi ut aliquip
                            ex ea commodo consequat. Duis aute irure dolor in
                            reprehenderit in voluptate velit esse cillum dolore
                            eu fugiat nulla pariatur. Excepteur sint occaecat
                            cupidatat non proident, sunt in culpa qui officia
                            deserunt mollit anim id est laborum.
                        </p>
                        <div
                            class="flex flex-col justify-center pt-6 sm:flex-row lg:justify-start"
                        >
                            <div
                                class="flex items-center justify-center sm:justify-start"
                            >
                                <p
                                    class="pt-2 text-md leading-relaxed text-black sm:text-md lg:text-md"
                                >
                                    Connect with us
                                </p>
                                <div class="hidden sm:block">
                                    <i
                                        class="bx bx-chevron-right text-2xl text-primary"
                                    ></i>
                                </div>
                            </div>
                            <div
                                class="flex items-center justify-center pt-5 pl-2 sm:justify-start sm:pt-0"
                            >
                                <a href="/">
                                    <i
                                        class="bx bxl-facebook-square text-2xl text-primary hover:text-yellow"
                                    ></i>
                                </a>
                                <a href="/" class="pl-4">
                                    <i
                                        class="bx bxl-twitter text-2xl text-primary hover:text-yellow"
                                    ></i>
                                </a>
                                <a href="/" class="pl-4">
                                    <i
                                        class="bx bxl-dribbble text-2xl text-primary hover:text-yellow"
                                    ></i>
                                </a>
                                <a href="/" class="pl-4">
                                    <i
                                        class="bx bxl-linkedin text-2xl text-primary hover:text-yellow"
                                    ></i>
                                </a>
                                <a href="/" class="pl-4">
                                    <i
                                        class="bx bxl-instagram text-2xl text-primary hover:text-yellow"
                                    ></i>
                                </a>
                            </div>
                        </div>
                    </div>
                    <div
                        class="w-full pl-0 pt-10 sm:w-3/4 lg:w-2/5 lg:pl-12 lg:pt-0"
                    >
                        <div>
                            <div class="flex items-end justify-between">
                                <h4
                                    class="font-body font-semibold uppercase text-black"
                                >
                                    Consultancy
                                </h4>
                                <h3
                                    class="font-body text-3xl font-bold text-primary"
                                >
                                    85%
                                </h3>
                            </div>
                            <div class="mt-2 h-3 w-full rounded-full bg-lila">
                                <div
                                    class="h-3 rounded-full bg-primary"
                                    style="width: 50%"
                                ></div>
                            </div>
                        </div>
                        <div class="pt-6">
                            <div class="flex items-end justify-between">
                                <h4
                                    class="font-body font-semibold uppercase text-black"
                                >
                                    Python
                                </h4>
                                <h3
                                    class="font-body text-3xl font-bold text-primary"
                                >
                                    70%
                                </h3>
                            </div>
                            <div class="mt-2 h-3 w-full rounded-full bg-lila">
                                <div
                                    class="h-3 rounded-full bg-primary"
                                    style="width: 70%"
                                ></div>
                            </div>
                        </div>
                        <div class="pt-6">
                            <div class="flex items-end justify-between">
                                <h4
                                    class="font-body font-semibold uppercase text-black"
                                >
                                    Javascript
                                </h4>
                                <h3
                                    class="font-body text-3xl font-bold text-primary"
                                >
                                    98%
                                </h3>
                            </div>
                            <div class="mt-2 h-3 w-full rounded-full bg-lila">
                                <div
                                    class="h-3 rounded-full bg-primary"
                                    style="width: 98%"
                                ></div>
                            </div>
                        </div>
                        <div class="pt-6">
                            <div class="flex items-end justify-between">
                                <h4
                                    class="font-body font-semibold uppercase text-black"
                                >
                                    Figma
                                </h4>
                                <h3
                                    class="font-body text-3xl font-bold text-primary"
                                >
                                    91%
                                </h3>
                            </div>
                            <div class="mt-2 h-3 w-full rounded-full bg-lila">
                                <div
                                    class="h-3 rounded-full bg-primary"
                                    style="width: 91%"
                                ></div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            <section class="container py-16 md:py-20 bg-white" id="services">
                <h2
                    class="text-[3.0rem] font-bold leading-[4rem] tracking-tight text-black text-center sm:text-[3.5rem] lg:text-[3.5rem]"
                >
                    Our Services
                </h2>
                <h3
                    class="pt-3 text-center text-md leading-relaxed text-black sm:text-2xl lg:text-md"
                >
                    Explore the comprehensive services Oris Express has to offer
                </h3>

                <div
                    class="grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:grid-cols-3 md:gap-2 md:pt-12 lg:grid-cols-4"
                >
                    <div
                        class="group rounded px-2 py-12 shadow hover:bg-primary"
                    >
                        <div
                            class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28"
                        >
                            <div class="hidden group-hover:block">
                                <img
                                    src="/assets/img/icon-development-white.svg"
                                    alt="development icon"
                                />
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
                                Oris Education
                            </h3>
                            <p
                                class="text-gray-600 pt-4 text-sm group-hover:text-white md:text-base"
                            >
                                Lorem ipsum dolor sit amet, consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>
                    <div
                        class="group rounded px-2 py-12 shadow hover:bg-primary"
                    >
                        <div
                            class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28"
                        >
                            <div class="hidden group-hover:block">
                                <img
                                    src="/assets/img/icon-content-white.svg"
                                    alt="content marketing icon"
                                />
                            </div>
                            <div class="block group-hover:hidden">
                                <img
                                    src="/assets/img/icon-content-black.svg"
                                    alt="content marketing icon"
                                />
                            </div>
                        </div>
                        <div class="text-center">
                            <h3
                                class="pt-8 text-lg font-semibold text-primary group-hover:text-accent lg:text-xl"
                            >
                                Oris Business Development
                            </h3>
                            <p
                                class="text-gray-600 pt-4 text-sm group-hover:text-white md:text-base"
                            >
                                Lorem ipsum dolor sit amet, consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>
                    <div
                        class="group rounded px-2 py-12 shadow hover:bg-primary"
                    >
                        <div
                            class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28"
                        >
                            <div class="hidden group-hover:block">
                                <img
                                    src="/assets/img/icon-mobile-white.svg"
                                    alt="Mobile Application icon"
                                />
                            </div>
                            <div class="block group-hover:hidden">
                                <img
                                    src="/assets/img/icon-mobile-black.svg"
                                    alt="Mobile Application icon"
                                />
                            </div>
                        </div>
                        <div class="text-center">
                            <h3
                                class="pt-8 text-lg font-semibold text-primary group-hover:text-accent lg:text-xl"
                            >
                                Oris Biomedical
                            </h3>
                            <p
                                class="text-gray-600 pt-4 text-sm group-hover:text-white md:text-base"
                            >
                                Lorem ipsum dolor sit amet, consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>
                    <div
                        class="group rounded px-2 py-12 shadow hover:bg-primary"
                    >
                        <div
                            class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28"
                        >
                            <div class="hidden group-hover:block">
                                <img
                                    src="/assets/img/icon-mobile-white.svg"
                                    alt="Mobile Application icon"
                                />
                            </div>
                            <div class="block group-hover:hidden">
                                <img
                                    src="/assets/img/icon-mobile-black.svg"
                                    alt="Mobile Application icon"
                                />
                            </div>
                        </div>
                        <div class="text-center">
                            <h3
                                class="pt-8 text-lg font-semibold text-primary group-hover:text-accent lg:text-xl"
                            >
                                Oris Handyman Services
                            </h3>
                            <p
                                class="text-gray-600 pt-4 text-sm group-hover:text-white md:text-base"
                            >
                                Lorem ipsum dolor sit amet, consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>
                </div>
            </section>
            <section class="container py-16 md:py-20" id="contact">
                <h2
                    class="text-[3.0rem] font-bold leading-[4rem] tracking-tight text-black text-center sm:text-[3.5rem] lg:text-[3.5rem]"
                >
                    Contact Oris Express
                </h2>
                <h4
                    class="pt-3 text-center text-md leading-relaxed text-black sm:text-2xl lg:text-md"
                >
                    Have Any Questions?
                </h4>
                <div class="mx-auto w-full pt-5 text-center sm:w-2/3 lg:pt-6">
                    <p class="font-body text-grey-10">
                        Lorem ipsum dolor sit amet consectetur adipiscing elit
                        hendrerit condimentum turpis nisl sem, viverra habitasse
                        urna ante lobortis fermentum accumsan. Viverra habitasse
                        urna ante lobortis fermentum accumsan.
                    </p>
                </div>
                <form class="mx-auto w-full pt-10 sm:w-3/4">
                    <div class="flex flex-col md:flex-row">
                        <input
                            class="mr-3 w-full rounded border-grey-50 px-4 py-3 font-body text-black md:w-1/2 lg:mr-5"
                            placeholder="Name"
                            type="text"
                            id="name"
                        />
                        <input
                            class="mt-6 w-full rounded border-grey-50 px-4 py-3 font-body text-black md:mt-0 md:ml-3 md:w-1/2 lg:ml-5"
                            placeholder="Email"
                            type="text"
                            id="email"
                        />
                    </div>
                    <textarea
                        class="mt-6 w-full rounded border-grey-50 px-4 py-3 font-body text-black md:mt-8"
                        placeholder="Message"
                        id="message"
                        cols="30"
                        rows="10"
                    ></textarea>
                    <button
                        class="mt-6 flex items-center justify-center rounded bg-primary px-8 py-3 font-header text-lg font-bold uppercase text-white hover:bg-grey-20"
                    >
                        Send
                        <i
                            class="bx bx-chevron-right relative -right-2 text-3xl"
                        ></i>
                    </button>
                </form>
                <div class="flex flex-col pt-16 lg:flex-row">
                    <div
                        class="w-full border-l-2 border-t-2 border-r-2 border-b-2 border-gray-300 px-4 py-4 sm:py-8 lg:w-1/3"
                    >
                        <div class="flex items-center">
                            <i class="bx bx-phone text-2xl text-grey-40"></i>
                            <p
                                class="pl-2 font-body font-bold text-grey-40 lg:text-lg"
                            >
                                Phone
                            </p>
                        </div>
                        <p
                            class="pt-2 text-left font-body font-bold text-primary lg:text-md"
                        >
                            (+233) 50 601 0209
                        </p>
                    </div>
                    <div
                        class="w-full border-l-2 border-t-0 border-r-2 border-b-2 border-gray-300 px-6 py-6 sm:py-8 lg:w-1/3 lg:border-l-0 lg:border-t-2"
                    >
                        <div class="flex items-center">
                            <i class="bx bx-envelope text-2xl text-grey-40"></i>
                            <p
                                class="pl-2 font-body font-bold text-grey-40 lg:text-lg"
                            >
                                Phone
                            </p>
                        </div>
                        <p
                            class="pt-2 text-left font-body font-bold text-primary lg:text-md"
                        >
                            (+233) 55 047 8180
                        </p>
                    </div>
                    <div
                        class="w-full border-l-2 border-t-0 border-r-2 border-b-2 border-gray-300 px-6 py-6 sm:py-8 lg:w-1/3 lg:border-l-0 lg:border-t-2"
                    >
                        <div class="flex items-center">
                            <i class="bx bx-map text-2xl text-grey-40"></i>
                            <p
                                class="pl-2 font-body font-bold text-grey-40 lg:text-lg"
                            >
                                Email
                            </p>
                        </div>
                        <p
                            class="pt-2 text-left font-body font-bold text-primary lg:text-md"
                        >
                            info@orisexpress.com
                        </p>
                    </div>
                </div>
            </section>
        </div>
    </MainLayout>
</template>
