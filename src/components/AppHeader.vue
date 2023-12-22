<script>
export default {
  name: "AppHeader",
  props: { links: Array },
};
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="/img/dc-logo.png" alt="" />
      </div>
      <nav class="menuNav">
        <ul>
          <li v-for="(link, i) in links" :key="i">
            <a href="" :class="link.current ? 'active' : ''">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;

header {
  background-color: white;
  margin: 20px 0 0;
  padding: 10px 0;
  .container {
    @include between();
    @include center(horizontal);

    ul {
      list-style: none;
      margin: 10px;
      @include center();
      li a {
        display: inline-block;
        padding: 1rem;
        text-decoration: none;
        font-weight: 500;
        font-size: 12px;
        &.active,
        &:hover {
          color: #0282f9;
          border-bottom: solid 5px #0282f9;
        }
      }
    }
  }
}
</style>
