<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
import AppListProduct from './components/AppListProduct.vue'

export default {
  components: {
    AppHeader,
    AppFooter,
    AppListProduct
  }
}
</script>

<template>
  <AppHeader />
  <AppListProduct />
  <AppFooter />
</template>

<style lang="scss">
@use 'styles/general' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap');
</style>
