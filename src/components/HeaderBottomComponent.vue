<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="jumbotron">
       <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
    .jumbotron {
        height: 450px;
        

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            }
        .container {
            max-width: $main-container;
            background-color: blue;
            height: 100%;
            margin: auto;
            position: relative;

            
        }
    }
</style>