<script>
import AppHeader from './components/AppHeader.vue'
import ListProducts from './components/ListProducts.vue'

export default {
  components: {
    AppHeader,
    ListProducts
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <ListProducts />
  </main>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;

a {
  color: $grey;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $light;
}
</style>
