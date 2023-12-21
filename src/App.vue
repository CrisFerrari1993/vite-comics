<script>
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader
  }
}
</script>

<template>
  <AppHeader />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primary;
}
</style>
