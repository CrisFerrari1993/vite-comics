<script>
export default {
    name: 'AppHeader',
}
</script>

<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li>
                    <a class="active" href="">
                        Prova
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
// SCSS ONLY COMPONENT
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.container {
    display: flex;
    justify-content: space-between;

    ul {
        list-style: none;
        @include center();


        li a {
            display: inline-block;
            padding: 2.5rem 1rem;
            text-decoration: none;
            font-weight: 600;


            &.active,
            &:hover {
                border-bottom: 3px solid #0282f9;
                color: #0282f9;
            }
        }
    }
}
</style>
