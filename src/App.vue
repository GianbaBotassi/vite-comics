<script>
import AppHeader from './components/AppHeader.vue'
import AppHero from './components/AppHero.vue'
import AppListProduct from './components/AppListProduct.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppHero,
    AppListProduct,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppHero />
  <AppListProduct />
  <AppFooter />
</template>

<style lang="scss">
@use 'styles/general' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap');
</style>
