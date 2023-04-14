<script>
export default {
    name: "appCard",
    props: {
        image: String,
        price: String,
        series: String,
        type: String

    }

}
</script>

<template>
    <div class="card">
        <img :src="image" alt="">
        <div class="bottom-card">
            <div class="name">{{ series }}</div>
            <div class="price">{{ price }}</div>
        </div>
    </div>
</template>

<style scope lang="scss">
img {
    max-width: 100%;
}
.card{
        width: calc(100% / 6 - 10px);
        padding: 5px;
        height: 200px;
        margin: 20px 0;
        img {
            object-fit: cover;
            height: 150px;
        }
        
        .bottom-card {

            .name {
                font-weight: 500;
            font-size: 0.7rem;
                
                text-align: center;
                color: white;
        }
        .price {
            font-size: 0.5rem;
            text-align: center;
            color: white;
        }
        }
    }
</style>