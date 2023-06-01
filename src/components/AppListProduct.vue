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
        <div id="product-container" class="container">
            <AppProduct v-for="(product, index) in myJson" :item="product" :key="index" />
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
    @include flex-content(center);
    flex-wrap: wrap;
    gap: 25px 15px;
    padding: 30px 0;
}
</style>