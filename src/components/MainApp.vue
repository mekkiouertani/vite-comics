<template>
    <div class="jumbotron">
        <img src="../../../images/jumbotron.jpg" alt="jumbotron">
    </div>
    <section>
        <div class="container">
            <div class="row gx-6 gy-3 align-content-center">
                <div class="col-12 col-md-4 col-lg-3" v-for="(card, index) in cards" :key="index">
                    <CardComponent :image="card.thumb" :title="card.series" />
                </div>
            </div>
        </div>
    </section>
    <TopMain />
    <BottomMain />
</template>

<script>
import BottomMain from "./MainComponents/BottomMain.vue";
import CardComponent from "./MainComponents/CardComponent.vue";
import TopMain from "./MainComponents/TopMain.vue";
import { cards } from "../data/dc-comics.js";

export default {
    name: "MainApp",
    components: { TopMain, BottomMain, CardComponent, cards },
    data() {
        return {
            cards: cards,
        };
    },
};
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.jumbotron {
    width: 100%;
    height: 400px;
    overflow: hidden;
}

section {
    padding: 20px;
    background-color: $dark-color;
}
</style>
