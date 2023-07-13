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
    <main>
    <div class="container">
      <h2>
        --> Content goes here &lt;--
      </h2>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/reset.scss" as *;

main {
    background-color: $main-gb;
    color: $main-txt;

    .container {
        max-width: $main-container;
        margin: auto;
        padding: 57px 0;
    }
}
</style>