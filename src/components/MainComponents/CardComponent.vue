<template>
    <div>
        <div class="cards">
            <div class="img-box">
                <img :src="image" :alt="title" />
            </div>
            <h5 class="text-white py-3 ">{{ title }}</h5>
        </div>
    </div>
</template>

<script>
export default {
    name: "CardComponent",
    props: ["image", "title"],
};
</script>
<style lang="scss" scoped>
.cards {
    width: 200px;


    .img-box {
        width: 200px;
        height: 200px;
        object-fit: cover;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
}
</style>
