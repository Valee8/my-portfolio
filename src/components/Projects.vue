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
    <section id="projects">
        <div class="section-left">
            <h2>
                <span>&lt;</span>Projects<span>&gt;</span>
            </h2>

            <p>
                You can see all the projects and repositories
                on my personal GitHub page.
            </p>
        </div>

        <div class="section-right">
            <div class="project" v-for="(projects, index) in listProjects" :key="index">
                <div class="project-content">
                    <h3>
                        {{ projects.title }}
                    </h3>

                    <p>
                        {{ projects.description }}
                    </p>

                    {{ projects.technologies }}
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;

section {
    display: flex;
    justify-content: space-between;

    .section-left {
        width: 28%;

        h2 {
            height: calc(100% - 30px);
        }
    }

    .section-right {
        width: 55%;

        .project {
            display: flex;
            align-items: center;
            background-color: #212023;
            width: 480px;
            border-radius: 4px;
            padding: 40px;

            h3 {
                font-size: 1.8rem;
                font-weight: 400;
            }

            p {
                font-weight: 300;
                line-height: 20px;
                font-size: 0.95rem;
                text-align: justify;
                color: #d7d6d7;
                padding: 10px 0;
            }

            &:first-child {
                margin-bottom: 15px;
            }

            &:last-child {
                margin-top: 15px;
            }
        }
    }
}
</style>
