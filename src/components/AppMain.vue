<script>
import Presentation from './Presentation.vue';

export default {
    name: 'AppMain',
    components: {
        Presentation
    }
}
</script>

<template>
    <Presentation />
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;
</style>
