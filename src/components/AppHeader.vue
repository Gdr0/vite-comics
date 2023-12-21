<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <h1>
    <header>
      <div class="container">
        <div class="logo">
          <img src="" alt="" />
        </div>
        <nav class="menuNav">
          <ul>
            <li>
              <a href="">dc</a>
            </li>
            <li>
              <a href="">dc</a>
            </li>
            <li>
              <a href="">dc</a>
            </li>
            <li>
              <a href="">dc</a>
            </li>
            <li>
              <a href="">dc</a>
            </li>
          </ul>
        </nav>
      </div>
    </header>
  </h1>
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;

header {
  background-color: white;
  margin: 20px 0;
  .container {
    width: 80%;
    margin: 0 auto;
    @include between();
    @include center(horizontal);

    ul {
      list-style: none;
      margin: 1px;
      @include center();
      li a {
        display: inline-block;
        padding: 1rem;
        text-decoration: none;
        font-weight: 300;
        font-size: 20px;
      }
    }
  }
}
</style>
