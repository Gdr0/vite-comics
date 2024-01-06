<script>
export default {
  name: "FooterFollow",
  props: {
    socials: Array,
  },
};
</script>
<template>
  <section>
    <div class="container">
      <div class="sign-up">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="social">
        <span> Follow us</span>
        <ul>
          <li v-for="(social, i) in socials" :key="i">
            <img :src="social.img" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@use "../styles/partials/_mixins.scss" as *;
section {
  background-color: #262626;
  .container {
    @include between();
    .sign-up {
      padding: 10px 0;
      @include center(horizontal);
      button {
        padding: 10px;
        background-color: #262626;
        color: white;
        border: 2px solid #0282f9;
        &:hover {
          cursor: pointer;
        }
      }
    }
    .social {
      padding: 10px 0;
      @include direction(row);
      align-items: center;
      gap: 15px;
      span {
        color: #0282f9;
        font-size: large;
        font-weight: bold;
        &:hover {
          cursor: pointer;
        }
      }
      ul {
        @include direction(row);
        gap: 10px;

        li {
          list-style: none;
          &:hover {
            cursor: pointer;
          }
          img {
            width: 30px;
          }
        }
      }
    }
  }
}
</style>
