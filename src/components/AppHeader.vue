<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            image: 'dc-logo.png',
            tools: [
                { text: 'CHARACTERS', url: '#' },
                { text: 'COMICS', url: '#' },
                { text: 'MOVIES', url: '#' },
                { text: 'TV', url: '#' },
                { text: 'GAMES', url: '#' },
                { text: 'COLLECTIBLES', url: '#' },
                { text: 'VIDEOS', url: '#' },
                { text: 'FANS', url: '#' },
                { text: 'NEWS', url: '#' },
                { text: 'SHOP', url: '#' },
            ]
        }
    },
    methods: {
        buildImg(image) {
            const url = new URL(`../assets/img/${image}`, import.meta.url);
            return url.href;
        }
    }
}
</script>

<template>
    <div class="container flex-header">
        <div>
            <figure>
                <img :src="buildImg(image)" alt="dc-logo">
            </figure>
        </div>
        <div>
            <nav>
                <ul>
                    <li v-for="voice in tools">
                        <a href="{{ voice.url }}">{{ voice.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.flex-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 15vh;
}

figure {
    width: 50px;
    cursor: pointer;
}

ul {
    display: flex;
    justify-content: space-between;
    list-style-type: none;

    li {
        a {
            text-decoration: none;
            color: #000;
            padding: 0.75rem;
            font-size: 0.70rem;
        }
    }
}

li a:hover {
    color: #0282F9;
    border-bottom: solid 3px #0282F9;
}
</style>