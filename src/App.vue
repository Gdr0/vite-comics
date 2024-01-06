<script>
import AppHeader from "./components/AppHeader.vue";
import ListProducts from "./components/ListProducts.vue";
import DcElementsList from "./components/DcElementsList.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  components: {
    AppHeader,
    ListProducts,
    DcElementsList,
    AppFooter,
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
      DCelements: [
        {
          text: "DIGITAL COMICS",
          img: "public/img/buy-comics-digital-comics.png",
          url: "#",
        },
        {
          text: "DC MERCHANDISE",
          img: "public/img/buy-comics-merchandise.png",
          url: "#",
        },
        {
          text: "SUBSCRIPTION",
          img: "public/img/buy-comics-subscriptions.png",
          url: "#",
        },
        {
          text: "COMIC SHOP LOCATOR",
          img: "public/img/buy-comics-shop-locator.png",
          url: "#",
        },
        {
          text: "DC POWER VISA",
          img: "public/img/buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <AppHeader :links="menu" />
  <ListProducts />
  <DcElementsList :links="DCelements" />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/general.scss" as *;
</style>
