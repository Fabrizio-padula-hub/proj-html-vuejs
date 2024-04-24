<script>
import AppHeader from './components/AppHeader.vue';
import AppProducts from './components/AppProducts.vue';
import AppSpecialMoments from './components/AppSpecialMoments.vue';
import AppShop from './components/AppShop.vue';
import AppProductViewing from './components/AppProductViewing.vue';
import AppCityWork from './components/AppCityWork.vue';
import AppGalleryImages from './components/AppGalleryImages.vue';
import AppDelivery from './components/AppDelivery.vue';
import AppFooter from './components/AppFooter.vue';

export default{
  components: {
    AppHeader,
    AppProducts,
    AppSpecialMoments,
    AppShop,
    AppProductViewing,
    AppCityWork,
    AppGalleryImages,
    AppDelivery,
    AppFooter
  },
  data(){
    return{
      navList: [
        { title: 'SHOP' },
        { title: 'ABOUT' },
        { title: 'GALLERY' },
        { title: 'LOCATIONS' },
        { title: 'JOURNAL' },
        { title: 'CONTACT' },
      ]
    }
  }
}
</script>

<template>

  <AppHeader :navList="navList"></AppHeader>

  <main>
    <AppProducts></AppProducts>
    <AppSpecialMoments></AppSpecialMoments>
    <AppShop></AppShop>
    <AppProductViewing></AppProductViewing>
    <AppCityWork></AppCityWork>
    <AppGalleryImages></AppGalleryImages>
    <AppDelivery></AppDelivery>
  </main>

  <AppFooter :navList="navList"></AppFooter>

</template>

<style lang="scss">
@use './style/generic';

</style>
