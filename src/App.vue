<template>
    <div id="all">
      <HeaderApp />
      <MainApp id="main"/>
      <FooterApp id="footer"/>
    </div>
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
#all{
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  #main{
    flex-grow: 1;
  }
}
  #footer{
    flex-grow: 1;
  }
</style>