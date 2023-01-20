<script>
import AppHeader from './components/AppHeader.vue';
import AppMainC from './components/AppMainContent.vue';
export default {
    data() {
        return {}
    },
    components: {
        AppHeader: AppHeader,
        AppMainC: AppMainC,
    }
}

</script>

<template>
    <app-header></app-header>
    <app-main-c></app-main-c>
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