<template>
    <TopMain/>
    <BottomMain/>
</template>

<script>
import BottomMain from './MainComponents/BottomMain.vue';
import TopMain from './MainComponents/TopMain.vue';

export default {
    name: "MainApp",
    components: { TopMain, BottomMain,},
    data() {
        return {
        }
    },
}
</script>

<style lang="scss" scoped>

</style>