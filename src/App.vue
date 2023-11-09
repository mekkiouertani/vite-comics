<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<script>
import FooterApp from './components/FooterApp.vue';
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';


export default {
  name: "App",
  components: { 
    HeaderApp, 
    FooterApp, 
    MainApp 
  }
}
</script>

<style lang="scss" scoped>

</style>