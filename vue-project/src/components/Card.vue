<script setup>
import { defineProps } from 'vue'

defineProps({
    bg: {
        type: String,
        default: "bg-white"
    },
    button: {
        type: String,
        default: "bg-blue-600 hover:bg-blue-700 text-white"
    }

});
</script>

<template>
    <div :class="`${bg} shadow-lg rounded-lg p-6`">
        <slot></slot>
    </div>
</template>