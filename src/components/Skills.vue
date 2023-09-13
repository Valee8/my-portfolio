<script>
export default {
    name: 'Projects',
    data() {
        return {
            listProjects: [
                {
                    title: "social-network",
                    description: "A project that aims to improve skills and learn new technologies. Initially, the focus is on learning and designing the business layer, not on the UI.",
                    technologies: "Typescript, React, Node.js"
                },
                {
                    title: "multilingual-json-split",
                    description: "Split the JSON into multiple files of each language",
                    technologies: "JavaScripts"
                },
                {
                    title: "jwt-auth",
                    description: "The focus is on learning and designing the business layer, not on the UI",
                    technologies: "Typescript, React, Node.js"
                }
            ]
        }
    }
}
</script>

<template>
    <section id="skills">
        <h2>
            <span>&lt;</span>Skills<span>&gt;</span>
        </h2>
    </section>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;
</style>
