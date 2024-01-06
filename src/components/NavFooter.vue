<script>
export default {
  name: "NavFooter",
  props: {
    voce: Array,
    links: Array,
  },
};
</script>
<template>
  <div class="backgaround">
    <div class="container">
      <div class="navList">
        <ul>
          <li v-for="(section, i) in voce" :key="i">
            <h3>{{ section.title }}</h3>
            <ul>
              <li v-for="(link, i) in section.links" :key="i">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;

.backgaround {
  background-image: url(public/img/footer-bg.jpg);
  .container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    .navList {
      color: white;
      width: calc(33.33% - 10px);
      margin-bottom: 10px;
      li {
        list-style-type: none;
        a {
          color: grey;
          text-decoration: none;
          font-size: small;
        }
      }
    }
  }
}
</style>
