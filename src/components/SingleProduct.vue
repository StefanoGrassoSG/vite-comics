<script>
export default {
    data() {
        return {

        }
    },
    props: {
        productImage: String,
        productName: String,
        productPrice: String
    }
}
</script>

<template>
    <div>
        <div class="img-card">
          <img :src="productImage" alt="">
        </div>
        <div class="title-card">
          {{ productName }}
        </div>
        <div class="price">
          {{ productPrice }}
        </div>
    </div>
</template>

<style lang="scss" scoped>
.img-card > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.title-card {
    padding: 5px 0;
    text-transform: uppercase;
}

.img-card {
    display: inline-block;
    width: 100%;
    height: 80%;
}
</style>