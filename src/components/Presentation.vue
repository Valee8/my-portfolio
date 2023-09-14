<script>
export default {
    name: 'Presentation',
}
</script>

<template>
    <section>
        <div class="section-left">
            <h1>
                Ciao,
                <div>sono Valerio</div>
            </h1>

            <h3>
                &lt;Full Stack Developer&gt;
                <div>with a passion for mobile development</div>
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem aspernatur et quod, magni fugit modi fuga
                similique voluptatum blanditiis, dolorum officia debitis tempore, molestiae temporibus.
            </p>

            <div class="buttons">
                <a href="/" class="button contact-me">
                    Contact me
                </a>
                <a href="/" class="button cv">
                    Download CV
                </a>
            </div>
        </div>

        <div class="section-right">
            <div class="image">

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
        width: 40%;

        h1 {
            font-size: 4rem;
            font-weight: 400;
            padding-bottom: 80px;
        }

        h3 {
            font-size: 1.5rem;
            font-weight: 400;
            padding-bottom: 20px;
        }

        p {
            line-height: 25px;
            font-weight: 300;
            color: #c8c9d0;
        }

        .buttons {
            padding-top: 50px;

            .button {
                //padding: 13px 30px;
                width: 200px;
                height: 60px;
                display: inline-block;
                text-align: center;
                line-height: 60px;
                border-radius: 5px;
                background-color: rgba(255, 255, 255, .05);
                font-weight: 300;

                &.contact-me {
                    border: 2px solid #059676;
                    color: #059676;
                    margin-right: 20px;
                }

                &.cv {
                    border: 2px solid #7a4ac8;
                    color: #7a4ac8;
                }
            }
        }
    }

    .section-right {
        width: 50%;
        padding-top: 60px;

        .image {
            background-color: #ccc;
            width: 360px;
            height: 440px;
        }
    }
}
</style>
