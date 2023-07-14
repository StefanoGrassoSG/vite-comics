<script>
export default {
    data() {
        return {
          icons: [
            'img/footer-facebook.png',
            'img/footer-youtube.png',
            'img/footer-periscope.png',
            'img/footer-pinterest.png',
            'img/footer-twitter.png'
          ]
        }
    },
    methods: {
      getImagePath: function(img) {
        return new URL(`../assets/${img}`, import.meta.url).href;
      }
    }
}
</script>

<template>
    <div class="footer-bottom">
    <div class="container">
      <div class="sign">
        <a href="">
          SIGN-UP NOW!
        </a>
      </div>

      <div class="follow">
        <h3>
          FOLLOW US
        </h3>
        <ul>
          <li v-for="singleIcon in icons">
            <a href="">
              <img :src=getImagePath(singleIcon) alt="">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/reset.scss" as *;

.footer-bottom {
    background-color: #2F2F2F;
    padding: 65px 0;

    .container {
        width: $main-container;
        margin: auto;
        display: flex;
        justify-content: space-between;
    }

    .sign > a {
        text-decoration: none;
        color: $main-txt;
        border: 2px solid #0282F9;
        padding: 20px;
        font-weight: bold;
    }

    .follow {
        display: flex;
        align-items: center;
    }

    .follow h3 {
        color: #0282F9;
    }

    ul {
        display: flex;
        list-style: none;
    }

    ul > li {
        margin-left: 15px;
    }
}
</style>