<script>
export default {
    name: 'AppMainC',
    data() {
        return {
            text: '-->CONTENT GOES HERE<--',
        }
    },
}
</script>

<template>
    <div class="bgc-custom">
        <div class="container content-main">
            <h2>{{ text }}</h2>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bgc-custom {
    background-color: #1C1C1C;

}

.content-main {
    color: #FDFCFC;
    height: 10vh;
    display: flex;

    h2 {
        align-self: center;
    }
}
</style>