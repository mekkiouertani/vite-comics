<template>
    <section>
        <div class="container d-flex justify-content-between p-5">
            <div class="right">
                <span>SIGN-UP NOW</span>
            </div>
            <div class="left d-flex align-items-center">
                <span >FOLLOW US</span>
                <img src="../../images/footer-facebook.png" alt="logo">
                <img src="../../images/footer-periscope.png" alt="logo">
                <img src="../../images/footer-pinterest.png" alt="logo">
                <img src="../../images/footer-twitter.png" alt="logo">
                <img src="../../images/footer-youtube.png" alt="logo">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "FooterApp"
}
</script>

<style lang="scss" scoped>
section{
    color: white;
    background-color: #1c1c1c;
}
.right{
    padding: 10px 20px;
    border: 2px solid #0282f9;
    cursor: pointer;
}
.left{
    img{
        height: 40px;
        width: 40px;
        margin: 0 5px;
        cursor: pointer;
    }
    span{
        color: #0282f9;
        font-weight: bold;
        font-size: 2rem;
        margin-right: 20px;
    }
}
    

</style>