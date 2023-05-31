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
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        <ul>
            <li v-for="link in links">
                {{ link.text }}
            </li>
        </ul>
    </header>
</template>

<style lang="scss">
@use 'styles/general' as *;
@use 'styles/partials/mixins' as *;

header {
    @include flex-content(between);
    margin-top: 20px;

    div {
        width: 50px;
        height: 50px;
    }

    ul {
        width: 60%;
        @include flex-content(center);
        gap: 5px;
    }
}
</style>
