<template>
    <div>
        <div class="card">
            <img :src="thumb" class="card-img-top" :alt="series">
            <div class="card-body">
                <h5 class="card-title">{{ series }} hellooo</h5>
            </div>
            
        </div>
    </div>
</template>

<script>
    export default {
        name: "CardComponent",
        props: [ "thumb", "series" ],
    }
</script>

<style lang="scss" scoped>

</style>