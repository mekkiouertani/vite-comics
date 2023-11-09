<template>
    <div class="container d-flex py-3">
        <div class="box-logo">
            <img src="../../public/images/dc-logo.png" alt="">
        </div>
        <ul class="d-flex">
            <li v-for="list in dataNav" class="px-3 list-group-item text-uppercase fw-bold">
            {{ list }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "HeaderApp",
    data(){
        return{
            dataNav: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fan",
                "news",
                "shop"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #444444;
}
.box-logo{
    width: 100px;
    height: 100px;
    img{
        max-width: 100%;
    }
}
li{
    &:hover{
        color: #0282f9;
        cursor: pointer;
        border-bottom: 1px solid #0282f9;
    }
}

</style>