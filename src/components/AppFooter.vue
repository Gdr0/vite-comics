<script>
import NavFooter from "./NavFooter.vue";
import FooterFollow from "./FooterFollow.vue";
export default {
  name: "AppFooter",
  components: {
    NavFooter,
    FooterFollow,
  },
  data() {
    return {
      DcLinks: [
        {
          title: "DC COMICS",
          links: [
            { text: "Characters", url: "#" },
            { text: "Comics", url: "#" },
            { text: "TV", url: "#" },
          ],
        },
        {
          title: "SHOP",
          links: [
            { text: "Shop DC", url: "#" },
            { text: "Shop DC Collectibles", url: "#" },
          ],
        },
        {
          title: "DC",
          links: [
            { text: "Terms Of Use", url: "#" },
            { text: "Privacy Policy (New)", url: "#" },
            { text: "Ad Choices", url: "#" },
            { text: "Advertising", url: "#" },
            { text: "Jobs", url: "#" },
            { text: "Subscriptions", url: "#" },
            { text: "Talent Workshops", url: "#" },
            { text: "CPSC Certificates", url: "#" },
            { text: "Ratings", url: "#" },
            { text: "Shop Help", url: "#" },
            { text: "Contact Us", url: "#" },
          ],
        },
        {
          title: "SITES",
          links: [
            { text: "DC", url: "#" },
            { text: "MAD Magazine", url: "#" },
            { text: "DC Kids", url: "#" },
            { text: "DC Universe", url: "#" },
            { text: "DC Power Visa", url: "#" },
          ],
        },
      ],
      SocialMedia: [
        {
          img: "public/img/footer-facebook.png",
          title: "Facebook",
          url: "#",
        },
        {
          img: "public/img/footer-periscope.png",
          title: "Periscope",
          url: "#",
        },
        {
          img: "public/img/footer-pinterest.png",
          title: "Pinterest",
          url: "#",
        },
        {
          img: "public/img/footer-twitter.png",
          title: "Twitter",
          url: "#",
        },
        {
          img: "public/img/footer-youtube.png",
          title: "YouTube",
          url: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <NavFooter :voce="DcLinks" />
  <FooterFollow :socials="SocialMedia" />
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
</style>
