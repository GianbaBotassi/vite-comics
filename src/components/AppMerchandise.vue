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
                <div class="merch-img">
                    <img :src="getImagePath(item.img)" alt="HELP">
                </div>
                <div>{{ item.text }}</div>

            </li>
        </ul>

    </div>
</template>

<style lang="scss">
@use 'styles/general' as *;
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

#merchandise {
    background-color: $blue;
    padding: 20px 0;

    ul {
        font-size: 0.5rem;
        color: $white-font;
        @include flex-content(around);

        li {
            @include flex-content;
            gap: 15px;

            img {
                height: 30px;
                width: 25px;
            }
        }
    }
}
</style>

