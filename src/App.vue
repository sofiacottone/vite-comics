<script>
import AppHeader from './components/AppHeader.vue';
import AppMainCards from './components/AppMainCards.vue';
import AppMainPages from './components/AppMainPages.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    components: {
        AppHeader,
        AppMainCards,
        AppMainPages,
        AppFooter
    }
}
</script>

<template>
    <AppHeader></AppHeader>

    <main>
        <AppMainCards></AppMainCards>
        <AppMainPages></AppMainPages>
    </main>

    <footer>
        <AppFooter></AppFooter>
    </footer>
</template>

<style lang="scss">
@use './style/generic';
</style>