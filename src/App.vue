<script>
import AppHeader from './components/AppHeader.vue';
import AppMainC from './components/AppMainContent.vue';
import AppMainN from './components/AppMainNav.vue';
import AppMainT from './components/AppMianTerms.vue';
export default {
    data() {
        return {}
    },
    components: {
        AppHeader: AppHeader,
        AppMainC: AppMainC,
        AppMainN: AppMainN,
        AppMainT: AppMainT,
    }
}

</script>

<template>
    <header>
        <app-header></app-header>
    </header>
    <main>
        <app-main-c></app-main-c>
        <app-main-n></app-main-n>
        <app-main-t></app-main-t>
    </main>
</template>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Open Sans;
    color: #000;
}

.container {
    max-width: 1048px;
    margin: 0 auto;
}

img {
    max-width: 100%;
}
</style>