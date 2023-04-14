<script>
export default {
    name: "AppFooter"
}
</script>

<template>
    <div class="footer-top">
        <div class="container">

        </div>
    </div>
    <div class="footer-bottom">
        <div class="container">
            <button class="footer-btn">SIGN-UP NOW!</button>
            <div class="icons">
                <div class="follow-us">FOLLOW-US</div>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixins" as *;

.footer-top {
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
}

.footer-bottom {
    height: 150px;
    background-color: $footer-color;

    .container {
        @include flex (row, space-between, center);
        .footer-btn {
            padding: 20px;
            border: 2px solid $primary-color;
            background-color: $footer-color;
            color: white;
            align-self: left;
        }
        .icons {
            @include flex (row, center, center);
            
            .follow-us {
            color: $primary-color;
            font-weight: 900;
            margin-right: 10px;
        }
        }
    }
    img {
               padding: 10px;
            }
}
</style>