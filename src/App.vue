<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMainContent from './components/AppMainContent.vue';
  import AppMainLinks from './components/AppMainLinks.vue';


  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppMainLinks,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <main>
    <AppMainContent></AppMainContent>
    <AppMainLinks></AppMainLinks>

  </main>

</template>

<style lang="scss">
  @use './style/generic'

</style>
