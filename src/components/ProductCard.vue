<script>
export default {
    name: 'ProductCard',
    props: {
        details: Object,
    }
}
</script>

<template>
    <div class="col">
        <a href="">
            <img :src="details.thumb" :alt="details.series">
            <h6>{{ details.series }}</h6>
        </a>
    </div>
</template>

<style lang="scss" scoped>
// SCSS ONLY COMPONENT
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.col {
    width: calc((100% / 6) - 1rem);
    margin: 0.5rem;
    text-align: center;

    a {
        text-decoration: none;

        img {
            height: 200px;
        }

        h6 {
            margin: 1rem 0;
            color: $light;
        }
    }

}
</style>