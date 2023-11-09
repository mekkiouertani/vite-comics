<template>
    <section id="top">
        <div class="container">
            <h5 class="text-white fs-3">Content Goes Here</h5>
        </div>
    </section>

    <section id="bottom">
        <div class="container">
            <ul class="w-100">
                <li v-for="item in dataBottomMain" class="list-group-item text-uppercase d-flex align-items-baseline">
                    <div class="box-item-logo">
                        <img :src="item.img" alt="item.name" class="w-100">
                    </div>
                    <p class="px-3 fs-6 fw-bold mt-4">{{ item.text }}</p>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "TopMain",
    data(){
        return{
            dataBottomMain: [
                {
                    text: "digital comics",
                    img : "../../../public/images/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    img : "../../../public/images/buy-comics-merchandise.png"
                },
                {
                    text: "subscritpion",
                    img : "../../../public/images/buy-comics-subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    img : "../../../public/images/buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    img : "../../../public/images/buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section{
    height: 150px;
    color: white;
}
#top{
    background-color: #1c1c1c;
}
#bottom{
    background-color: #0282f9;
}
.container{
    height: 100%;
    display: flex;
    align-items: center;
}
.box-item-logo{
    width: 50px;
    height: 50px;
}
ul{
    display: flex;
    justify-content: space-between;
}
</style>