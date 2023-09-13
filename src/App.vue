<script>
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import AppNav from './components/AppNav.vue';


export default {
  components: {
    AppFooter,
    AppMain,
    AppNav
  }
}
</script>

<template>
  <div id="main-container">
    <AppNav />

    <div class="main-footer">
      <main>
        <div class="container">
          <AppMain />
        </div>
      </main>

      <AppFooter />
    </div>
  </div>
</template>

<style lang="scss">
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;

#main-container {
  display: flex;

  .main-footer {
    width: calc(100% - 230px);
  }
}
</style>
