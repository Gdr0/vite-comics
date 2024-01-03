<script>
export default {
  name: "DcElementsList",
  props: { links: Array },
};
</script>

<template>
  <div>
    <div class="container">
      <ul>
        <li v-for="(link, i) in links" :key="i">
          <a :href="link.url">{{ link.text }}</a>
          <img :src="link.img" />
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
div {
  background-color: #0282f9;
  ul {
    list-style: none;

    padding: 30px;
    @include center();
    gap: 30px;
    li {
      @include center();
    }
    li a {
      display: inline-block;
      padding: 1rem;
      text-decoration: none;
      font-weight: bold;
      font-size: 10px;
      color: white;
    }
    li img {
      width: 40px;
    }
  }
}
</style>
