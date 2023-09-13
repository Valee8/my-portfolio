<script>
export default {
    name: 'AppNav',
    data() {
        return {
            navLinks: [
                {
                    text: "Projects",
                    link: "#projects"
                },
                {
                    text: "Skills",
                    link: "#skills"
                },
                {
                    text: "Experience",
                    link: "#"
                },
                {
                    text: "Contact",
                    link: "#"
                }
            ],
            navSocials: [
                {
                    text: "Linkedin",
                    link: "",
                    icon: "fa-brands fa-linkedin"
                },
                {
                    text: "GitHub",
                    link: "",
                    icon: "fa-brands fa-github"
                }
            ]
        }
    }
}
</script>

<template>
    <nav>
        <div class="top-nav">
            Jr. Full Stack Web Developer
        </div>

        <div class="center-nav">
            <ul class="nav-links">
                <li v-for="(links, index) in navLinks" :key="index">
                    <a :href="links.link">
                        {{ links.text }}
                    </a>
                </li>

            </ul>
        </div>

        <div class="bottom-nav">
            <ul class="nav-socials">
                <li v-for="(socials, index) in navSocials" :key="index">
                    <a :href="socials.link">
                        <i :class="socials.icon" class="icon-socials"></i> {{ socials.text }}
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;

nav {
    display: flex;
    flex-direction: column;
    background-color: #111111;
    width: 230px;
    height: 100vh;
    font-size: 0.85rem;
    padding: 15px 0;

    div {
        display: flex;
        justify-content: center;
        align-items: center;

        &.top-nav {
            width: 125px;
            align-self: flex-end;
            text-align: right;
            padding-right: 20px;
        }

        &:nth-child(2) {
            flex-grow: 1;

            .nav-links {
                width: 100%;

                li {
                    margin: 0 4px;
                    text-align: center;
                    height: 40px;
                    line-height: 40px;
                    border-bottom: 1px solid #1d1d1d;

                    &:last-child {
                        border-bottom: 0;
                    }
                }
            }
        }

        .nav-socials {
            li {
                padding: 5px 0;
                font-size: 0.9rem;

                .icon-socials {
                    font-size: 1.2rem;
                    vertical-align: middle;
                    padding-right: 6px;
                }
            }
        }
    }

    // .container {
    //     display: flex;
    //     justify-content: space-between;
    //     align-items: center;

    //     .nav-links {
    //         display: flex;
    //         justify-content: space-between;
    //         align-items: center;
    //         gap: 20px;
    //     }
    // }
}
</style>
