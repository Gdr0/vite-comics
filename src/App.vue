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
  data() {
    return {
      menu: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Video",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <AppHeader :links="menu" />
  <ListProducts />
  <DcElementsList />
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/general.scss" as *;
</style>
