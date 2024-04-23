<script>
import AppHeader from './components/AppHeader.vue';
import AppProducts from './components/AppProducts.vue';
import AppSpecialMoments from './components/AppSpecialMoments.vue';

export default{
  components: {
    AppHeader,
    AppProducts,
    AppSpecialMoments
  }
}
</script>

<template>

  <AppHeader></AppHeader>

  <main>
    <AppProducts></AppProducts>
    <AppSpecialMoments></AppSpecialMoments>

  </main>

</template>

<style lang="scss">
@use './style/generic';

</style>
