<script>
export default {
    name: 'Presentation',
}
</script>

<template>
    <section>
        <h1>
            Ciao,
            <div>sono Valerio</div>
        </h1>
    </section>
</template>

<style lang="scss" scoped>
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/mixins' as *;
@use '../src/styles/partials/variables' as *;

section {
    h1 {
        font-size: 4rem;
        font-weight: 400;
    }
}
</style>
