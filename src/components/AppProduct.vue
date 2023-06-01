<script>
export default {
    name: "AppProduct",
    props: {
        item: Object            //riferimento a item in AppListProduct (padre)
    }
}
</script>

<template>
    <a class="card" href="#">
        <div>
            <img :src="item.thumb" :alt="item.series"> <!-- uso item come riferimento per prendere dall'oggetto -->
        </div>
        <h6>{{ item.series }}</h6>
    </a>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

.card {
    flex-basis: calc((100%/6) - 15px);
    height: 150px;

    img {
        height: 120px;
        width: 100px;
    }

    h6 {
        margin-top: 5px;
    }
}
</style>