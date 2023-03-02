<script>
import AppNav from './AppNav.vue'

export default {
  name: 'AppHeader',
  components: {
    AppNav
  }
}
</script>

<template>
  <header>
    <AppNav />
  </header>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;
</style>
