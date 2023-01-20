<script>
export default {
    name: 'AppMainT',
    data() {
        return {
            image: 'dc-logo-bg.png',
            comics: [
                { text: 'CHARACTERS', url: '#' },
                { text: 'COMICS', url: '#' },
                { text: 'MOVIES', url: '#' },
                { text: 'TV', url: '#' },
                { text: 'GAMES', url: '#' },
                { text: 'VIDEOS', url: '#' },
                { text: 'NEWS', url: '#' },
            ],
            shop: [
                { text: 'SHOP DC', url: '#' },
                { text: 'SHOP DC COLLECTIBLES', url: '#' },
            ],
            dc: [
                { text: 'TERMS OF USE', url: '#' },
                { text: 'PRIVACY POLICI (NEW)', url: '#' },
                { text: 'AD CHOICES', url: '#' },
                { text: 'ADVERTISING', url: '#' },
                { text: 'JOBS', url: '#' },
                { text: 'SUBSCRIPTIONS', url: '#' },
                { text: 'TALENT WORKSHOP', url: '#' },
                { text: 'CPSC CERTIFICATION', url: '#' },
                { text: 'RATINGS', url: '#' },
                { text: 'SHOP HELP', url: '#' },
                { text: 'CONTACT US', url: '#' },
            ],
            sites: [
                { text: 'DC', url: '#' },
                { text: 'MAD MAGAZINE', url: '#' },
                { text: 'DC KIDS', url: '#' },
                { text: 'DC UNIVERSE', url: '#' },
                { text: 'DC POWER VISA', url: '#' },
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
    <div class="bgi-custom">
        <div class="container flex-header">
            <div class="list-flex">
                <nav>
                    <ul>
                        <h3>DC COMICS</h3>
                        <li v-for="voice in comics">
                            <a href="{{ voice.url }}">{{ voice.text }}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3>SHOP</h3>
                        <li v-for="voice in shop">
                            <a href="{{ voice.url }}">{{ voice.text }}</a>
                        </li>
                    </ul>
                </nav>
                <nav>
                    <ul>
                        <h3>DC</h3>
                        <li v-for="voice in dc">
                            <a href="{{ voice.url }}">{{ voice.text }}</a>
                        </li>
                    </ul>
                </nav>
                <nav>
                    <ul>
                        <h3>SITES</h3>
                        <li v-for="voice in sites">
                            <a href="{{ voice.url }}">{{ voice.text }}</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <div>
                <figure>
                    <img :src="buildImg(image)" alt="dc-logo">
                </figure>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bgi-custom {
    background-image: url(../assets/img/footer-bg.jpg);
}

.flex-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 55vh;
}

.list-flex {
    display: flex;
    justify-content: space-between;
}

ul {
    list-style-type: none;
    padding: 1rem;

    h3 {
        color: #FDFCFC;
    }

    li {
        a {
            text-decoration: none;
            color: #949494;
            font-size: 0.70rem;
        }
    }
}

figure {
    width: 350px;
    cursor: pointer;
}

li a:hover {
    color: #FDFCFC;
    box-shadow: 0px 1px 2px #FDFCFC;
}
</style>