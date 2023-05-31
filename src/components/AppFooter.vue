<script>
export default {
    name: "AppFooter",
    data() {
        return {
            items: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png'
                }
            ]
        }
    }
}
</script>

<template>
    <div id="merchandise">
        <ul class="container">
            <li>
                ciao
            </li>
            <li>
                ciao
            </li>
            <li>
                ciao
            </li>
            <li>
                ciao
            </li>
            <li>
                ciao
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
        @include flex-content(around)
    }
}
</style>

