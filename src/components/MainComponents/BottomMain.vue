<template>
    <section>
        <div class="container d-flex justify-content-between">
            <div class="left">
                <ul class="mt-3">
                    <li v-for="(item, index) in itemsBottomMain" :key="index" class="list-group-item">
                        <h4 class="text-uppercase">{{ item.title }}</h4>
                        <div v-for="(list, index) in itemsBottomMain" class="text-secondary">
                            {{ list.listItems[index] }}
                        </div>
                    </li>
                </ul>
            </div>
            <div class="right">
                <img src="../../../images/dc-logo-bg.png" alt="">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "BottomMain",
    data(){
        return{
            itemsBottomMain: [
            {
                title: "dc comics",
                listItems: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                ],
            },
            {
                title: "shop",
                listItems: [
                    "Characters",
                    "Comics",
                ],
            },
            {
                title: "dc",
                listItems: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                ],
            },
            {
                title: "sites",
                listItems: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                ],
            },
        ]
        }
        
    }
}
</script>

<style lang="scss" scoped>
section{
    background-image: url(../../../public/images/footer-bg.jpg);
    height: 400px;
    overflow: hidden;
    color: white;
}
ul{
    width: 500px;
    display: flex;
    flex-wrap: wrap;
    li{
        padding: 20px 30px 0px 20px;
    }
}
</style>