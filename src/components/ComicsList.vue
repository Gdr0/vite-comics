<script>
export default {
  name: "ComicsList",
};
</script>
<template>
  <div class="container">
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
    </div>
    <div class="card-comic">
      <img
        src="https://www.coverbrowser.com/image/action-comics/1-1.jpg"
        alt=""
      />
      <span class="title">Action comics</span>
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
      font-size: 12px;
      font-weight: bold;
    }
  }
}
</style>
