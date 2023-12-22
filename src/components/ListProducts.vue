<script>
import DcJumbo from "./DcJumbo.vue";
export default {
  name: "ListProducts",
  components: {
    DcJumbo,
  },
};
</script>

<template>
  <DcJumbo />
</template>

<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
h2 {
  color: white;
}
</style>
