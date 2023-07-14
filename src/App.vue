<script >
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import ShopbarComponent from './components/ShopbarComponent.vue';
import FootertopComponent from './components/FootertopComponent.vue';
import FooterbottomComponent from './components/FooterbottomComponent.vue';
import HeaderBottomComponent from './components/HeaderBottomComponent.vue';

export default {
  data() {
    return {

    }
  },
  methods: {

  },
  components: {
    HeaderComponent,
    MainComponent,
    ShopbarComponent,
    FootertopComponent,
    FooterbottomComponent,
    HeaderBottomComponent
  }
}
</script>

<template>

  <HeaderComponent />

  <HeaderBottomComponent />

  <MainComponent />

  <ShopbarComponent />

 
  <FootertopComponent />
  <FooterbottomComponent />


</template>

<style lang="scss">
@use "assets/scss/main";
@use "assets/scss/partials/reset";
</style>
