<script>
export default {
  name: "ComicsList",
  props: { comics: Array },
};
</script>
<template>
  <div class="container">
    <div v-for="(comic, i) in comics" :key="i" class="card-comic">
      <img :src="comic.thumb" />
      <span class="title">{{ comic.series }}</span>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
.container {
  @include center();
  flex-wrap: wrap;
  background-color: #1c1c1c;

  .card-comic {
    @include direction(column);
    width: calc((100% / 6) - 20px);
    margin: 20px 10px;
    img {
      width: 100%;
    }
    span {
      color: white;
      font-size: 15px;
      font-weight: bold;
      margin-top: 10px;
    }
    &:hover {
      cursor: pointer;
    }
  }
}
</style>
