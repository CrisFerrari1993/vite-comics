<script>
export default {
    name: 'AppFooter',
    data() {
        return {

        }
    }
}
</script>

<template>
    <footer>
        <section class="main">
            <div class="container">

            </div>
        </section>
        <section class="secondary">

        </section>
    </footer>
</template>

<style lang="scss" scoped>
// SCSS ONLY COMPONENT
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

footer {
    section.main {
        background-image: url('../../public/img/social/footer-bg.jpg');
        background-size: cover;
    }
}
</style>