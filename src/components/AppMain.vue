<script>
import Presentation from './Presentation.vue';
import Projects from './Projects.vue';
import Skills from './Skills.vue';
import Experience from './Experience.vue';
import Contact from './Contact.vue';

export default {
    name: 'AppMain',
    components: {
        Presentation,
        Projects,
        Skills,
        Experience,
        Contact
    }
}
</script>

<template>
    <Presentation />
    <Projects />
    <Skills />
    <Experience />
    <Contact />
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;
</style>
