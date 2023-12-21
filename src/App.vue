<script>
import AppHeader from "./components/AppHeader.vue";
import ListProducts from "./components/ListProducts.vue";
import DcElementsList from "./components/DcElementsList.vue";
export default {
  components: {
    AppHeader,
    ListProducts,
    DcElementsList,
  },
};
</script>

<template>
  <AppHeader />
  <ListProducts />
  <DcElementsList />
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/general.scss" as *;
</style>
