<template>
    <div>
        <Link :href="route('home')">Home</Link>
        <Link :href="route('sobre')">Sobre</Link>
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