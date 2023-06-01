<script>
export default {
    name: "AppMerchandise",
    data() {
        return {
            items: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png',
                    url: '#',
                    current: false
                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png',
                    url: '#',
                    current: false
                },
                {
                    text: 'SUBSCRIPTION',
                    img: 'buy-comics-subscriptions.png',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png',
                    url: '#',
                    current: false
                },
                {
                    text: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.svg',
                    url: '#',
                    current: false
                },
            ]
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <div id="merchandise">
        <ul class="container">
            <li v-for="item in items">
                <a :href="item.url">
                    <div class="merch-img">
                        <img :src="getImagePath(item.img)" :alt="item.text">
                    </div>
                    <div>{{ item.text }}</div>
                </a>

            </li>
        </ul>

    </div>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

#merchandise {
    background-color: $blue;
    padding: 20px 0;

    ul {
        font-size: 0.5rem;
        color: $white-font;
        @include flex-content(around);

        li a {
            @include flex-content;
            height: 30px;
            gap: 15px;

            .merch-img {
                width: 30px;
            }
        }
    }
}
</style>

