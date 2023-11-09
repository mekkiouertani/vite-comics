<template>
    <div class="container d-flex py-3">
        <div class="box-logo">
            <img src="../../images/dc-logo.png" alt="">
        </div>
        <ul>
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
    margin-left: 30px;
    min-width: 100px;
    height: 100px;
    img{
        max-width: 100%;
    }
}
ul{
    display: flex;
    justify-content: end;
    flex-wrap: wrap;
    gap: 5px;
}
li{
    &:hover{
        color: #0282f9;
        cursor: pointer;
        border-bottom: 1px solid #0282f9;
    }
}

</style>