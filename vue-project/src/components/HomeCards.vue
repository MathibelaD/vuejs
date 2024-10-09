<script setup>
import Card from './Card.vue'
</script>

<template>
    <section class="py-20 bg-gray-100">
        <div class="container mx-auto text-center">
            <h2 class="text-3xl font-bold mb-10">Welcome to FreelanceHub</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Influencer Card -->
                <Card>
                    <h3 class="text-xl font-semibold mb-2">For Influencers</h3>
                    <p class="text-gray-600 mb-4">
                        Discover amazing freelance gigs tailored for influencers and showcase your unique skills.
                    </p>
                    <div class="flex justify-end">
                        <a href="#" class="bg-blue-600 hover:bg-blue-700 text-white py-2 px-4 rounded">
                            Browse Gigs
                        </a>
                    </div>
                </Card>

                <!-- Client Card -->
                <div class="bg-white shadow-lg rounded-lg p-6">
                    <h3 class="text-xl font-semibold mb-2">For Clients</h3>
                    <p class="text-gray-600 mb-4">
                        Post your gigs and connect with talented influencers ready to take your projects to the next
                        level.
                    </p>
                    <div class="flex justify-end">
                        <a href="#" class="bg-blue-600 hover:bg-blue-700 text-white py-2 px-4 rounded">
                            Post a Gig
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
/* Optional additional styles can go here */
</style>