<template>
    <section class="min-h-screen">
        <div
            class="container flex flex-col items-center py-16 md:py-20 lg:flex-row"
        >
            <div class="w-full text-center sm:w-3/4 lg:w-3/5 lg:text-left">
                <SectionHeader
                    title="Who we are?"
                    subTitle="A comprehensive solutions expert"
                    class="text-left"
                    classSub="text-left"
                />
                <p class="pt-6 font-body leading-relaxed text-gray-20">
                    Welcome to Oris Express, your trusted partner in educatoinal
                    and business consultancy and engineering solutions. Our
                    company is dedicated to providing comprehensive and
                    innovative services that cater to the needs, ensuring
                    excellence and satisfaction for all our clients.
                </p>
                <p class="pt-6 font-body leading-relaxed text-gray-20">
                    At Oris Express, we specialize in two main areas:
                    Consultancy and Engineering.
                </p>
                <h4 class="font-bold mt-6">Consultancy Services</h4>
                <p class="pt-2 font-body leading-relaxed text-gray-20">
                    Education Services: We offer expert guidance and support in
                    the education sector, helping institutions improve their
                    strategies, curriculum, and overall effectiveness. Our team
                    of seasoned professionals is committed to driving
                    educational excellence and fostering a culture of continuous
                    improvement.
                </p>
                <p class="pt-2 font-body leading-relaxed text-gray-20">
                    Business Development Management: Our consultancy services
                    extend to helping businesses grow and thrive. We provide
                    strategic insights, market analysis, and practical solutions
                    to enhance business performance and achieve sustainable
                    growth. Whether you are a startup or an established
                    enterprise, we have the expertise to take your business to
                    the next level.
                </p>
                <h4 class="font-bold mt-6">Engineering Services</h4>
                <p class="pt-2 font-body leading-relaxed text-gray-20">
                    Biomedical Engineering: Our engineering division excels in
                    biomedical engineering, where we combine innovation and
                    technical expertise to develop advanced medical devices and
                    solutions. Our goal is to improve patient care and
                    healthcare outcomes through cutting-edge technology and
                    engineering prowess.
                </p>
                <p class="pt-2 font-body leading-relaxed text-gray-20">
                    Handyman Services: We also offer reliable handyman services,
                    addressing various maintenance and repair needs with
                    precision and professionalism. Our skilled technicians are
                    equipped to handle a wide range of tasks, ensuring your
                    property remains in excellent condition.
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
            <div class="w-full pl-0 pt-10 sm:w-3/4 lg:w-2/5 lg:pl-12 lg:pt-0">
                <div>
                    <div class="flex items-end justify-between">
                        <h4
                            class="font-body font-semibold uppercase text-black"
                        >
                            Consultancy
                        </h4>
                        <h3 class="font-body text-3xl font-bold text-primary">
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
                        <h3 class="font-body text-3xl font-bold text-primary">
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
                        <h3 class="font-body text-3xl font-bold text-primary">
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
                        <h3 class="font-body text-3xl font-bold text-primary">
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
</template>

<script setup lang="ts">
import SectionHeader from "./SectionHeader.vue";
</script>

<style scoped></style>
