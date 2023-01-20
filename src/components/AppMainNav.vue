<script>
export default {
    name: 'AppMainN',
    data() {
        return {
            navs: [
                { text: 'DIGITAL COMICS', url: '#' },
                { text: 'DC MERCHANDISE', url: '#' },
                { text: 'SUBSCRIPTION', url: '#' },
                { text: 'COMIC SHOP LOCATOR', url: '#' },
                { text: 'DC POWER VISA', url: '#' },
            ]
        }
    },
}
</script>

<template>
    <div class="bgc-custom">
        <div class="container flex-main-c">
            <nav>
                <ul>
                    <li v-for="(voice, i) in navs">
                        <a href="{{ voice.url }}">{{ voice.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bgc-custom {
    background-color: #0282F9;

}

nav {
    height: 15vh;

    ul {
        display: flex;
        justify-content: space-between;
        list-style-type: none;

        li {
            margin-top: 2.5rem;

            a {
                text-decoration: none;
                color: #FDFCFC;
                padding: 0.75rem;
                font-size: 0.80rem;
                align-self: center;

            }
        }
    }
}

li a:hover {
    text-shadow: 0px 1px 5px #FDFCFC;
}
</style>