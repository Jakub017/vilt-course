<template>
    <Link href="/">Go to Index view</Link><br />
    <Link href="/show">Go to Show view</Link>
    <div>Page time: {{ timer }}</div>
    <slot></slot>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
import { ref } from "vue";

const timer = ref(0);
setInterval(() => {
    timer.value++;
}, 1000);
</script>
