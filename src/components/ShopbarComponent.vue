<script>
export default {
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<template>
    <section>
    <nav>
      <ul>
        <li>
          <a href="">
            <div class="buy">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            </div>
            <span>DIGITAL COMICS</span>
          </a>
        </li>
        <li>
          <a href="">
            <div class="buy">
              <img src="../assets/img/buy-comics-merchandise.png" alt="">
            </div>
            <span>DC MERCHANDISE</span>
          </a>
        </li>
        <li>
          <a href="">
            <div class="buy">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            </div>
            <span>SUBSCRIPTION</span>
          </a>
        </li>
        <li>
          <a href="">
            <div class="buy">
              <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            </div>
            <span>COMIC SHOP LOCATOR</span>
          </a>
        </li>
        <li>
          <a href="">
            <div class="buy">
              <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            </div>
            <span>DC POWER VISA</span>
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