<script>
import json from '../json/dc-comics.json'
import AppProduct from './AppProduct.vue'


export default {
    name: "AppListProduct",
    components: {
        AppProduct,
    },
    data() {
        return {
            myJson: json
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <span id="current-series">CURRENT SERIES</span>
            <div id="product-container">
                <AppProduct v-for="(product, index) in myJson" :item="product" :key="index" />
                <!-- Ciclo product dal Json importato, legandolo al figlio con :item="product" -->
            </div>
            <div id="load-more">
                <span>LOAD MORE</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

section {
    background-color: $dark-grey;
    padding-bottom: 20px;

    .container {
        position: relative;

        span {
            background-color: $blue;
            color: $white-font;
            padding: 5px 20px;
        }

        #current-series {
            position: absolute;
            left: 0;
            top: -15px
        }

        #product-container {
            @include flex-content(center);
            flex-wrap: wrap;
            gap: 25px 15px;
            padding: 30px 0;
        }

        #load-more {
            font-size: 0.5rem;
            text-align: center;
            cursor: pointer;
        }
    }
}
</style>