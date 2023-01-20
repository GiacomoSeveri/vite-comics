<script>
export default {
    name: 'AppFooter',
    data() {
        return {}
    },
}
</script>

<template>
    <div class="bgc-custom">
        <div class="container flex-footer">
            <div>
                <button>SING-UP NOW!</button>
            </div>
            <div class="flex-footer">
                <a href="#">FOLLOW US</a>
                <figure>
                    <a href='#'><img src="../assets/img/footer-facebook.png" alt="facebook-logo"></a>
                    <a href='#'><img src="../assets/img/footer-twitter.png" alt="twitter-logo"></a>
                    <a href='#'><img src="../assets/img/footer-youtube.png" alt="youtube-logo"></a>
                    <a href='#'><img src="../assets/img/footer-pinterest.png" alt="pinterest-logo"></a>
                    <a href='#'><img src="../assets/img/footer-periscope.png" alt="periscope-logo"></a>
                </figure>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bgc-custom {
    background-color: #303030;
}

.flex-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 10vh;
}

button {
    background-color: #303030;
    padding: 12px 20px;
    color: #F1F9E4;
    border: solid 3px #0282F9;
    cursor: pointer;
}

a {
    color: #0282F9;
    font-size: 15px;
    font-weight: 900;
    text-decoration: none;
    margin: 0 7px;

    img {
        width: 30px;
    }
}

button:hover {
    text-shadow: 0px 1px 5px #FDFCFC;
}
</style>