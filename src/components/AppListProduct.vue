<script>
export default {
    name: "AppListProduct",
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div id="product-container" class="container">
            <a class="card" href="#">
                <div>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                </div>
                <h6>Ciaooooo</h6>
            </a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

section {
    background-color: $dark-grey;
}

#product-container {
    background-color: red;
    @include flex-content(center);
    flex-wrap: wrap;
    gap: 5px;

    .card {
        background-color: aqua;
        height: 150px;
        flex-basis: calc((100%/6) - 5px);

        div {
            text-align: center;
        }


    }
}
</style>