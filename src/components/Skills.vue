<script>
export default {
    name: 'Projects',
    data() {
        return {
            listSkills: [
                {
                    name: "nodejs",
                    icon: "fa-brands fa-node",
                },
                {
                    name: "git",
                    icon: "",
                },
                {
                    name: "javascript",
                    icon: "fa-brands fa-js",
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

        <div class="list-skills">
            <div class="skill" :class="skill.name" v-for="(skill, index) in listSkills" :key="index">
                <span class="icon" :class="{ 'none': skill.icon === '' }"><i :class="skill.icon"></i></span>
                <span class="name">&num;{{ skill.name }}</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;

section {
    .list-skills {
        display: flex;
        padding-top: 50px;

        .skill {
            display: flex;
            align-items: center;
            gap: 0 10px;
            font-weight: 400;
            border-radius: 4px;
            padding: 10px 20px;
            font-size: 1.4rem;
            margin: 5px;

            .icon {
                font-size: 1.6rem;

                &.none {
                    display: none;
                }
            }

            &.nodejs {
                background-color: #66b35d;
                color: #f0f1f9;

                .icon {
                    color: #3c5250;
                }
            }

            &.git {
                background-color: #f0f1f9;
                color: #0b243d;
            }

            &.javascript {
                background-color: #33a668;
                color: #f7df1e;
            }
        }

    }
}
</style>
