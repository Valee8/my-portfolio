<script>
import Presentation from './Presentation.vue';
import Projects from './Projects.vue';
import Skills from './Skills.vue';

export default {
    name: 'AppMain',
    components: {
        Presentation,
        Projects,
        Skills
    }
}
</script>

<template>
    <Presentation />
    <Projects />
    <Skills />
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;
</style>
