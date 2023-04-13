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

        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
.footer-top{
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
}
.footer-bottom {
    height: 150px;
    background-color: $footer-color;
}
</style>