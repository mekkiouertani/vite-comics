<template>
    <div id="all-top-main">

        <section id="top">
            <div class="container px-5">
                
            </div>
        </section>

        <section id="bottom">
            <div class="container ">
                <ul class="w-100">
                    <li v-for="item in dataBottomMain" class=" text-uppercase d-flex align-items-baseline">
                        <div class="box-item-logo">
                            <img :src="item.img" alt="item.name" class="w-100">
                        </div>
                        <p class="px-3 fs-6 fw-bold mt-4">{{ item.text }}</p>
                    </li>
                </ul>
            </div>
        </section>
    </div>
</template>

<script>
import {cards} from './../../data/dc-comics.js';
import CardComponent from '../MainComponents/CardComponent/CardComponent.vue'
export default {
    component : { cards, CardComponent},
    
    data(){
        return{
            dataBottomMain: [
                {
                    text: "digital comics",
                    img : "../../../images/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    img : "../../../images/buy-comics-merchandise.png"
                },
                {
                    text: "subscritpion",
                    img : "../../../images/buy-comics-subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    img : "../../../images/buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    img : "../../../images/buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
#top-all-main{
    display: flex;
    flex-grow: 1;
}
section{
    min-height: 120px;
    color: white;
}
#top{
    background-color: #1c1c1c;
}
#bottom{
    background-color: #0282f9;
}
.container{
    min-height: 100px;
    display: flex;
    align-items: center;
}
.box-item-logo{
    width: 50px;
    cursor: pointer;
}
ul{
    min-height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}
</style>