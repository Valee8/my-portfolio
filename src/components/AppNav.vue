<script>
export default {
    name: 'AppNav',
    data() {
        return {
            navLinks: [
                {
                    text: "Projects",
                    link: "#"
                },
                {
                    text: "Skills",
                    link: "#"
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
                        <i :class="socials.icon"></i> {{ socials.text }}
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
    width: 180px;
    height: 600px;
    font-weight: 300;

    a {
        font-size: 0.85rem;

    }

    div {
        display: flex;
        justify-content: center;
        align-items: center;

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

                    a {
                        //width: 100%;
                        //display: block;
                        color: #bbbbbb;
                    }
                }
            }
        }

        &:nth-child(3) {
            align-items: flex-end;
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
