<script>
export default {
    name: "AppHeader",
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
    <header class="container">
        <div>
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        <ul>
            <li v-for="link in links" :class="{ active: link.current }">
                {{ link.text }}
            </li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

header {
    @include flex-content(between);
    height: 100px;

    img {
        width: 70px;
        height: 70px;
    }

    ul {
        font-size: 0.7rem;
        font-weight: 500;
        @include flex-content(center);
        gap: 15px;
        height: 100%;

        li {
            height: 50px;
            @include flex-content(center);
            border-bottom: 3px solid transparent;
            height: 100%;

            &.active {
                border-bottom: 3px solid $blue;
                color: $blue;
            }
        }
    }
}
</style>
