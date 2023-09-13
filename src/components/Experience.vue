<script>
export default {
    name: 'Experience',
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
    <section id="experience">
        <h2>
            <span>&lt;</span>Work Experience<span>&gt;</span>
        </h2>

        <div class="list-experiences">
            <div class="experience">
                <div class="content-left">
                    <span class="date">
                        Jun 2020 - Jul 2021
                    </span>
                </div>


                <div class="content-right">
                    <span class="role">
                        Full Stack Developer
                    </span>
                    <h3>
                        Educational Environment
                    </h3>
                    <p>
                        Initially, single handedly led the effort to create the backend services for our web
                        application.
                        Developed
                        server side
                        logic, built a database design, created a template and a parser for an Excel file with a
                        schedule.
                        Deployed
                        the
                        server on
                        DigitalOcean, configured GitLab CI.
                        Performed coaching of interns developers joining the team, reviewed code, and referred them to a
                        possible
                        solution
                        while working with a senior engineer to define roadmap and feature priorities.
                        Managed communication with developer teams remotely and was in charge of estimation and
                        prioritization.
                    </p>

                    <div class="technologies">
                        Node.js, Express, Passport.js (later Firebase Auth), PostgreSQL, GitLab CI.
                    </div>
                </div>
            </div>

            <div class="experience">
                <div class="content-left">
                    <span class="date">
                        Jun 2020 - Jul 2021
                    </span>
                </div>


                <div class="content-right">
                    <span class="role">
                        Full Stack Developer
                    </span>
                    <h3>
                        Social network
                    </h3>
                    <p>
                        A project that aims to improve skills and learn new technologies. Initially, the focus is on
                        learning and designing the
                        business layer, not on the UI. Get experience with JWT and GraphQL (Apollo).
                    </p>

                    <div class="technologies">
                        React, Redux, Formik, Node.js, Express, Apollo, GraphQL, JWT
                    </div>
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
    .list-experiences {

        .experience {
            display: flex;
            gap: 0 30px;
            padding-top: 60px;
        }

        .content-left {
            .date {
                color: #d7d6d7;
            }
        }

        .content-right {
            width: 65%;

            h3 {
                color: #9a5bff;
                font-weight: 300;
                font-size: 2rem;
                padding: 10px 0;
            }

            p {
                border-left: 3px solid #cacad1;
                padding: 5px 5px 5px 20px;
                color: #d7d6d7;
                line-height: 25px;
            }

            .technologies {
                padding-top: 10px;
            }
        }
    }
}
</style>
