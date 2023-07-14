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
  <footer>
    <div class="footer-top">
      <div class="links">
        <div class="col-1">
          <h3>
            DC COMICS
          </h3>
          <ul>
            <li>
              <a href="">Characters</a>
            </li>
            <li>
              <a href="">Comics</a>
            </li>
            <li>
              <a href="">Movies</a>
            </li>
            <li>
              <a href="">Tv</a>
            </li>
            <li>
              <a href="">Games</a>
            </li>
            <li>
              <a href="">Videos</a>
            </li>
            <li>
              <a href="">News</a>
            </li>
          </ul>
          <h3>
            SHOP
          </h3>
          <ul>
            <li>
              <a href="">Shop DC</a>
            </li>
            <li>
              <a href="">Shop DC Collectibles</a>
            </li>
          </ul>
        </div>
        <div class="col-2">
          <h3>
            DC
          </h3>
          <ul>
            <li>
              <a href="">Terms Of Use</a>
            </li>
            <li>
              <a href="">Privacy policy(New)</a>
            </li>
            <li>
              <a href="">
                Ad choices
              </a>
            </li>
            <li>
              <a href="">Advertising</a>
            </li>
            <li>
              <a href="">Jobs</a>
            </li>
            <li>
              <a href="">Subscriptions</a>
            </li>
            <li>
              <a href="">Talent Workshops</a>
            </li>
            <li>
              <a href="">CPSC Certificates</a>
            </li>
            <li>
              <a href="">Ratings</a>
            </li>
            <li>
              <a href="">Shop Help</a>
            </li>
            <li>
              <a href="">Contact Us</a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <h3>
            SITES
          </h3>
          <ul>
            <li>
              <a href="">DC</a>
            </li>
            <li>
              <a href="">MAD Magazine</a>
            </li>
            <li>
              <a href="">DC Kids</a>
            </li>
            <li>
              <a href="">DC Universe</a>
            </li>
            <li>
              <a href="">DC Power Visa</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="big-logo">
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/reset.scss" as *;

footer {
    background-image: url('/src/assets/img/footer-bg.jpg');
    background-size: cover;
}
.footer-top {
        width: $main-container;
        margin: auto;
        display: flex;
        justify-content: space-between;
    }

    h3 {
        margin-top: 15px;
        margin-bottom: 15px;
        color: $main-txt;
    }

    li {
        margin-bottom: 5px;
    }

    li > a {
        color: $links-cl;
        text-decoration: none;
    }

    li > a:hover {
        color: $main-txt;
        text-decoration: underline $main-txt;
    }

    .links {
        display: flex;
        padding: 20px 0;
    }

    .links ul {
        list-style: none;
        padding: 0;
    }

    .col-1, .col-2, .col-3 {
        margin-right: 20px;
    }

    .big-logo {
        width: 40%;
        background-size: cover;
        background-position: center;
        background-image: url('/src/assets/img/dc-logo-bg.png');
    }
</style>