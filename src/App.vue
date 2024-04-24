<script>
import AppHeader from './components/AppHeader.vue';
import AppProducts from './components/AppProducts.vue';
import AppSpecialMoments from './components/AppSpecialMoments.vue';
import AppShop from './components/AppShop.vue';
import AppProductViewing from './components/AppProductViewing.vue';
import AppCityWork from './components/AppCityWork.vue';
import AppGalleryImages from './components/AppGalleryImages.vue';
import AppDelivery from './components/AppDelivery.vue';

export default{
  components: {
    AppHeader,
    AppProducts,
    AppSpecialMoments,
    AppShop,
    AppProductViewing,
    AppCityWork,
    AppGalleryImages,
    AppDelivery
  }
}
</script>

<template>

  <AppHeader></AppHeader>

  <main>
    <AppProducts></AppProducts>
    <AppSpecialMoments></AppSpecialMoments>
    <AppShop></AppShop>
    <AppProductViewing></AppProductViewing>
    <AppCityWork></AppCityWork>
    <AppGalleryImages></AppGalleryImages>
    <AppDelivery></AppDelivery>

  </main>

</template>

<style lang="scss">
@use './style/generic';

</style>
