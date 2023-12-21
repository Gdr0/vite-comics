<script>
export default {
  name: "AppHeader",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: false,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: true,
        },
        {
          text: "Video",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="" alt="" />
      </div>
      <nav class="menuNav">
        <ul>
          <li v-for="link in links">
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
  margin: 20px 0;
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
          color: #4941fe;
        }
      }
    }
  }
}
</style>
