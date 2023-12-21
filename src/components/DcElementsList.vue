<script>
export default {
  name: "DcElementsList",
};
</script>

<template>
  <div>
    <div class="container">
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
        <li>
          <a href="">dc</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
div {
  background-color: #4941fe;
  ul {
    list-style: none;
    margin: 40px;
    padding: 30px;
    @include center();
    gap: 30px;
    li a {
      display: inline-block;
      padding: 1rem;
      text-decoration: none;
      font-weight: 300;
      font-size: 20px;
    }
  }
}
</style>
