<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<template>
  <div class="container">
    <AppHeader />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use 'styles/general' as *;
@use 'styles/partials/mixins' as *;

.container {
  max-width: 1160px;
  margin: 0 auto;
  width: 70%;
}
</style>
