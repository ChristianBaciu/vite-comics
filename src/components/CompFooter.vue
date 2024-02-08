<script>
import { h } from 'vue';

export default{
    name: "CompFooter",
    components: { h }
}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>

<header>
    <nav>
        <div class="button">
            <h3>SIGN-UP NOW!</h3>
        </div>

        <div class="social">
            <h3>FOLLOW US</h3>
            <figure>
                <img src="../assets/img/footer-facebook.png" alt="logo">
                <img src="../assets/img/footer-twitter.png" alt="logo">
                <img src="../assets/img/footer-youtube.png" alt="logo">
                <img src="../assets/img/footer-pinterest.png" alt="logo">
                <img src="../assets/img/footer-periscope.png" alt="logo">
            </figure>
        </div>
    </nav>
</header>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{
    height: 12vh;
    background-color: #303030;
    position: relative;
    z-index: 999;
    display: flex;
    text-align: center;

    nav{
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 80%;
        margin: 0 auto;
        .button{
            border: 2px solid #1265b3;
            color: white;
            padding: 7px;
        }
        .social{
            display: flex;
            align-items: center;
            h3{
                color: #1265b3;
                padding-right: 20px;
            }
        }
        figure{
            display: flex;
            gap: 20px;
        }
    }
}
</style>
