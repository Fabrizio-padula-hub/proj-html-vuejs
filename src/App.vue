<script>
import AppHeader from './components/AppHeader.vue';
import AppProducts from './components/AppProducts.vue';
import AppSpecialMoments from './components/AppSpecialMoments.vue';
import AppShop from './components/AppShop.vue';

export default{
  components: {
    AppHeader,
    AppProducts,
    AppSpecialMoments,
    AppShop
  }
}
</script>

<template>

  <AppHeader></AppHeader>

  <main>
    <AppProducts></AppProducts>
    <AppSpecialMoments></AppSpecialMoments>
    <AppShop></AppShop>

  </main>

</template>

<style lang="scss">
@use './style/generic';

</style>
