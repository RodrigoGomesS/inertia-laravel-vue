<template>
    <div class="bg-gradient-to-tr from-indigo-600 to-purple-600 text-white">
        <Link class="py-2 px-3" :class="{ 'font-bold': $page.url === '/home' }" :href="route('home')">Home</Link>
        <Link class="py-2 px-3" :class="{ 'font-bold': $page.url === '/sobre' }" :href="route('sobre')">Sobre</Link>
    </div>
</template>

<script>
import { Link } from '@inertiajs/vue3';

export default {
    name: 'MenuNavBar',
    components: {
        Link
    },
}

</script>

<style lang="css" scoped></style>