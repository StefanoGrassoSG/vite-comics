<script>
export default {
    data() {
        return {
          allLinks: [
            {
              title: 'DC comics',
              links: [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Videos',
                'News'
              ]
            },
            {
              title: 'Shop',
              links: [
                'Shop DC',
                'Shop DC Collectibles'
              ]
            },
            {
              title: 'DC',
              links: [
                'Terms Of Use',
                'Privacy policy(New)',
                'Ad choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
              ]
            },
            {
              title: 'SITES',
              links: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
              ]
            }
          ]
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
            {{ allLinks[0].title }}
          </h3>
          <ul>
            <li v-for="singleLink in allLinks[0].links" >
              <a href="">{{ singleLink }}</a>
            </li>
          </ul>
          <h3>
            {{ allLinks[1].title }}
          </h3>
          <ul>
            <li v-for="singleLink in allLinks[1].links">
              <a href="">{{ singleLink }}</a>
            </li>
          </ul>
        </div>
        <div class="col-2">
          <h3>
            {{ allLinks[2].title }}
          </h3>
          <ul>
            <li v-for="singleLink in allLinks[2].links">
              <a href="">{{ singleLink }}</a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <h3>
            {{ allLinks[3].title }}
          </h3>
          <ul>
            <li v-for="singleLink in allLinks[3].links">
              <a href="">{{ singleLink }}</a>
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