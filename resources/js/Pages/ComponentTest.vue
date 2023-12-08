<script setup>
import GuestLayout from "@/Layouts/GuestLayout.vue";
import InputLabel from "@/Components/InputLabel.vue";
import TextInput from "@/Components/TextInput.vue";
// import { reactive } from "vue";
// import { Inertia } from "@inertiajs/inertia";

// defineProps({
//     errors: Object,
// });

// const form = reactive({
//     title: null,
//     content: null,
// });

// const submitFunction = () => {
//     Inertia.post("/inertia", form);
// };
</script>

<template>
    <GuestLayout>
        <InputLabel value="件名">タイトル</InputLabel>
        <TextInput modelValue="初期値"></TextInput>
    </GuestLayout>
</template>
