<script>
export default {
  name: "DcJumbo",
};
</script>

<template>
  <div class="jumbo"></div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
h2 {
  @include center();
  color: white;
}
.jumbo {
  width: 100%;
  height: 40vh; /* Altezza di esempio */
  background-image: url("/img/jumbotron.jpg");
  background-size: cover;
}
</style>
