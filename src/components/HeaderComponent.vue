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
     <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="">

      <nav>
        <ul>
          <li>
            <a href="">
              CHARACTERS
            </a>
          </li>
          <li>
            <a href="">
              COMICS
            </a>
          </li>
          <li>
            <a href="">
              MOVIES
            </a>
          </li>
          <li>
            <a href="">
              TV
            </a>
          </li>
          <li>
            <a href="">
              GAMES
            </a>
          </li>
          <li>
            <a href="">
              COLLECTIBLES
            </a>
          </li>
          <li>
            <a href="">
              VIDEOS
            </a>
          </li>
          <li>
            <a href="">
              FANS
            </a>
          </li>
          <li>
            <a href="">
              NEWS
            </a>
          </li>
          <li>
            <a href="">
              SHOP
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/reset.scss" as *;

header {
    background-color: $header-bg;
    padding: 12px 0;

    .container {
        max-width: $main-container;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    
        nav ul > * {
            display: inline-block;
        }

        li > a {
            text-decoration: none;
            color: #1C1C1C;
            font-weight: bold;
            padding: 50px 10px;
        }

        li > a:hover {
            border-bottom: 5px solid #0282F9;
            color: #0282F9;
        }
    }    
} 
</style>