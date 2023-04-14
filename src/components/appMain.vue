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
            <img :src="image" alt="">
            <div class="bottom-card">
                <div class="name">{{ series }}</div>
                <div class="price">{{ price }}</div>
            </div>


        </div>
    </div>
</template>

<style lang="scss" scoped>
.main {
    background-color: black;
    height: 200px;

    h4 {
        font-size: 2rem;
        color: white;
        line-height: 200px;
    }
}
</style>