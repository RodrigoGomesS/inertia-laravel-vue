<template>
    <Head :title="title" />
    <header>
        <MenuNavBar />
    </header>
    <main>
        <slot />
    </main>
</template>

<script setup>
import { Head } from '@inertiajs/vue3';
import MenuNavBar from '../Components/MenuNavBar.vue';

defineProps({
    title: String,
});

</script>