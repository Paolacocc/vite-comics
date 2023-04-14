<script>
import { stringifyExpression } from '@vue/compiler-core';

export default {
    name: "appMain",

    props: {
        image: String,
        price: String,
        series: String,
        type: String

    }
}
</script>

<template>
    <div class="main">
        <div class="container">
            <div class="card">
                <img :src="image" alt="">
                <div class="bottom-card">
                    <div class="name">{{ series }}</div>
                    <div class="price">{{ price }}</div>
                </div>
            </div>


        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/mixins" as *;
.main {
    background-color: black;
    height: 200px;

    .card{
        width: calc(100% / 6 - 10px);
    }
}
</style>