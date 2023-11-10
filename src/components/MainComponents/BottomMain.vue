<template>
    <section>
        <div class="container d-flex justify-content-between p-0">
            <div class="left">
                <ul class="mt-1">
                    <li v-for="(item, index) in itemsBottomMain" :key="index">
                        <h4 class="text-uppercase">{{ item.title }}</h4>
                        <div v-for="(list, index) in itemsBottomMain[index].listItems" class="text-secondary">
                            {{ list }}
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
                    "Games",
                    "Video",
                    "News",
                ],
            },
            {
                title: "dc",
                listItems: [
                "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Games",
                    "Video",
                    
                    
                ],
            },
            {
                title: "sites",
                listItems: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Characters",
                    "Comics",
                    "Movies",
                   
                    
                ],
            },
            {
                title: "shop",
                listItems: [
                    "Characters",
                    "Comics",

                ],
            },
        ]
        }
        
    }
}
</script>

<style lang="scss" scoped>
section{
    background-image: url(../../../images/footer-bg.jpg);
    overflow: hidden;
    color: white;
    max-height: 400px;
}
ul{
    width: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: start;
    align-content: start;
    align-items: start;
    
    li{
        padding: 20px 30px 0px 20px;
    }
}
</style>