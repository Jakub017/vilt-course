<template>
    <Link href="/">Go to Index view</Link><br />
    <Link href="/show">Go to Show view</Link>

    <slot></slot>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
</script>
