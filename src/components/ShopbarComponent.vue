<script>
export default {
    data() {
        return {
          links: [
            {
              name: 'DIGITAL COMICS',
              img: "img/buy-comics-digital-comics.png"
            },
            {
              name: 'DC MERCHANDISE',
              img: "img/buy-comics-merchandise.png"
            },
            {
              name: 'SUBSCRIPTION',
              img: "img/buy-comics-subscriptions.png"
            },
            {
              name: 'COMIC SHOP LOCATOR',
              img: "img/buy-comics-shop-locator.png"
            },
            {
              name: 'DC POWER VISA',
              img: "img/buy-dc-power-visa.svg"
            }
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
    <section>
    <nav>
      <ul>
        <li v-for="singleLink in links">
          <a href="">
            <div class="buy">
              <img :src=getImagePath(singleLink.img) alt="">
            </div>
            <span>{{ singleLink.name }}</span>
          </a>
        </li>
      </ul>
    </nav>
  </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/reset.scss" as *;

section {
    background-color: $nav-bg;

    nav {
        max-width: $main-container;
        margin: auto;
        padding: 50px 20px;
    }

    ul {
        display: flex;
        justify-content: space-between;
        list-style: none;
    }

    .buy {
        width: 60px;
        height: 60px;
    }

    a {
        display: flex;
        align-items: center;
        text-decoration: none;
        color: $main-txt;
    }

    .buy > img {
        width: 100%;
        height: 100%;
        object-fit: contain;
    }
}
</style>