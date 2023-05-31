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
    <div id="content">
      Content goes here </div>
  </div>
  <AppFooter />
</template>

<style lang="scss">
@use 'styles/general' as *;
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap');

.container {
  font-family: 'Roboto', sans-serif;
  max-width: 1160px;
  margin: 0 auto;
  width: 70%;
}

#content {
  background-color: black;
  height: 100px;
  color: $white-font;
  @include flex-content();
  padding-left: 20px;
}
</style>
