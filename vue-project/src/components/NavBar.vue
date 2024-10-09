<script setup>
// You can add any necessary logic here in the future
</script>

<template>
    <nav class="bg-gray-900 p-4">
        <div class="container mx-auto flex justify-between items-center">
            <!-- Logo -->
            <div class="flex">
                <img src="../assets/logo.svg" alt="logo image" class="h-5 mx-2" />
                <a href="#" class="text-white text-xl font-bold">FreelanceHub</a>
            </div>
            <!-- Nav Links -->
            <ul class="flex space-x-6">
                <li>
                    <a href="#" class="text-gray-300 hover:text-white">Home</a>
                </li>
                <li>
                    <a href="#" class="text-gray-300 hover:text-white">Browse Gigs</a>
                </li>
                <li>
                    <a href="#" class="text-gray-300 hover:text-white">Post a Gig</a>
                </li>
            </ul>

            <!-- Login/Signup -->
            <div>
                <a href="#" class="text-gray-300 hover:text-white mr-4">Log In</a>
                <a href="#" class="bg-blue-600 hover:bg-blue-700 text-white py-2 px-4 rounded">
                    Sign Up
                </a>
            </div>
        </div>
    </nav>
</template>

<style scoped>
/* Optionally add extra styles here */
</style>
