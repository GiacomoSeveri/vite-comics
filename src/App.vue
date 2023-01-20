<script>
import AppHeader from './components/AppHeader.vue';
export default {
    data() {
        return {}
    },
    components: {
        AppHeader: AppHeader,
    }
}

</script>

<template>
    <app-header></app-header>
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
</style>