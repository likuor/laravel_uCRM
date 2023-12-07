<script setup>
import { Link } from "@inertiajs/inertia-vue3";
</script>

<template>
    Inertia test
    <br />
    <a href="">a tag</a>
    <br />
    <Link href="">Link</Link>
    <br />
    <Link :href="route('inertia.index')">name route</Link>
    <br />
    <Link :href="route('inertia.show', { id: 1 })"
        >Line parameter name route</Link
    >
</template>
