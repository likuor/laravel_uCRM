<script setup>
import { Link } from "@inertiajs/inertia-vue3";
import { ref } from "vue";

const newTitle = ref("");
const newContent = ref("");
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

    <div class="mb-8"></div>
    <input type="text" name="newTitle" v-model="newTitle" /> {{ newTitle }}
    <br />
    <input type="text" name="newContent" v-model="newContent" />
    {{ newContent }}
    <br />
    <Link
        method="post"
        as="button"
        :href="route('inertia.store')"
        :data="{
            title: newTitle,
            content: newContent,
        }"
    >
        DB保存テスト</Link
    >
</template>
