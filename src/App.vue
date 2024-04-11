<script>
import AppHeader from './components/AppHeader.vue';
import AppMainCards from './components/AppMainCards.vue';
import AppMainPages from './components/AppMainPages.vue';

export default {
    components: {
        AppHeader,
        AppMainCards,
        AppMainPages,
    }
}
</script>

<template>
    <AppHeader></AppHeader>

    <main>
        <AppMainCards></AppMainCards>
        <AppMainPages></AppMainPages>
    </main>
</template>

<style lang="scss">
@use './style/generic';
</style>