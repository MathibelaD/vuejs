<script setup>
import { ref, onMounted, defineProps } from 'vue';
import gigsData from '../gigListing.json'

const gigs = ref([]);

defineProps({
    limit: Number,
});
onMounted(() => {
    gigs.value = gigsData;
});
</script>

<template>
    <section class="py-20 bg-gray-50">
        <div class="container mx-auto text-center">
            <h2 class="text-3xl font-bold mb-10">Browse Gigs</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div v-for="gig in gigs.slice(0, limit || gigs.lenth)" :key="gig.id"
                    class="bg-white shadow-lg rounded-lg p-6">
                    <h3 class="text-xl font-semibold mb-2">{{ gig.title }}</h3>
                    <p class="text-gray-600 mb-4">{{ gig.description }}</p>
                    <p class="font-medium mb-2">Tech Stack:</p>
                    <ul class="mb-4">
                        <li v-for="tech in gig.techStack" :key="tech"
                            class="inline-block bg-blue-200 rounded-full px-3 py-1 text-sm text-blue-800 mr-2">
                            {{ tech }}
                        </li>
                    </ul>
                    <p class="font-medium mb-2">Owner:</p>
                    <p>{{ gig.owner.name }}</p>
                    <p class="text-gray-600">{{ gig.owner.email }}</p>
                    <p class="text-gray-600">{{ gig.owner.phone }}</p>
                    <a href="#"
                        class="mt-4 block bg-blue-600 hover:bg-blue-700 text-white py-2 px-4 rounded text-center">
                        Learn More
                    </a>
                </div>
            </div>


            <a href="#" v-if="limit < gigs.length"
                class="mt-10 inline-block bg-green-600 hover:bg-green-700 text-white py-3 px-6 rounded">
                View All Gigs
            </a>
        </div>
    </section>
</template>

<style scoped>
/* Optional additional styles can go here */
</style>
