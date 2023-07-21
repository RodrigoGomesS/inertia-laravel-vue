<template>
    <header>
        <MenuNavBar />
    </header>
    <main>
        <slot />
    </main>
</template>

<script>
import MenuNavBar from '../Components/MenuNavBar.vue';
export default {
    components: {
        MenuNavBar
    },
}
</script>