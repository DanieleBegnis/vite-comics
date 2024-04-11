<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMainContent from './components/AppMainContent.vue';
  import AppMainLinks from './components/AppMainLinks.vue';
  import AppFooterLinks from './components/AppFooterLinks.vue';


  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppMainLinks,
      AppFooterLinks,
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

</template>

<style lang="scss">
  @use './style/generic'

</style>
