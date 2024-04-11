<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMainContent from './components/AppMainContent.vue';
  import AppMainLinks from './components/AppMainLinks.vue';
  import AppFooterLinks from './components/AppFooterLinks.vue';
  import AppFooterFinal from './components/AppFooterFinal.vue';


  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppMainLinks,
      AppFooterLinks,
      AppFooterFinal,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <main>
    <AppMainContent></AppMainContent>
    <AppMainLinks></AppMainLinks>
  </main>
  <AppFooterLinks></AppFooterLinks>
  <AppFooterFinal></AppFooterFinal>

</template>

<style lang="scss">
  @use './style/generic'

</style>
