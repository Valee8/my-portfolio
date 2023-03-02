<script>
export default {
    name: 'AppNav'
}
</script>

<template>
    <nav>
        <div class="container">
            <h1>
                Logo
            </h1>

            <ul class="nav-links">
                <li>
                    <a href="#">
                        About
                    </a>
                </li>
                <li>
                    <a href="#">
                        Projects
                    </a>
                </li>
                <li>
                    <a href="#">
                        Contacts
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
    background-color: rgba(0, 0, 0, .2);
    padding: 20px 0;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .nav-links {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
        }
    }
}
</style>
