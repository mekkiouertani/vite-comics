<template>
        <TopMain/>
        <BottomMain/>
</template>

<script>
import BottomMain from './MainComponents/BottomMain.vue';
import TopMain from './MainComponents/TopMain.Vue';

export default {
    name: "MainApp",
    components: { TopMain, BottomMain }
}
</script>

<style lang="scss" scoped>

</style>