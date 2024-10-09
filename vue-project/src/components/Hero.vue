<script setup>
import { defineProps } from 'vue'

defineProps({
    title: {
        type: String,
        default: 'Find Your Next Gig',
    }
});
</script>

<template>
    <section class="bg-gray-800 text-white py-10">
        <div class="container mx-auto flex flex-col md:flex-row items-center">
            <!-- Left Side: Text -->
            <div class="md:w-1/2 text-center md:text-left">
                <h1 class="text-4xl md:text-5xl font-bold mb-4">
                    {{ title }}
                </h1>
                <p class="text-lg mb-6">
                    Join our platform to explore amazing freelance opportunities or post your gigs and connect with
                    talented freelancers.
                </p>
                <a href="#" class="bg-blue-600 hover:bg-blue-700 text-white py-2 px-4 rounded">
                    Get Started
                </a>
            </div>
            <!-- Right Side: Image -->
            <div class="md:w-1/2 mt-8 md:mt-0">
                <img src="../assets/logo.svg" alt="Hero Image" class="w-full h-auto" />
            </div>
        </div>
    </section>
</template>

<style scoped>
/* Optional additional styles can go here */
</style>