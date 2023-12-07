<script setup>
import { reactive } from "vue";
import { Inertia } from "@inertiajs/inertia";
const form = reactive({
    title: null,
    content: null,
});

const submitFunction = () => {
    Inertia.post("/inertia", form);
};
</script>

<template>
    <form @submit.prevent="submitFunction" action="">
        <input name="title" type="text" v-model="form.title" />
        <br />
        <input name="content" type="text" v-model="form.content" />
        <br />
        <button>送信</button>
    </form>
</template>
