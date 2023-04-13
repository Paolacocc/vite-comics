<script>
export default {
    name: "appHeader",
    data(){
        return{
            navigationList: {
                text: "Characters"
            }
        }
    }
    

}
</script>

<template>
    <img src="../assets/img/dc-logo.png" alt="">

    <ul class="nav-list">
        <li class="list">{{ navigationList.text }}</li>
    </ul>
</template>

<style lang="scss" scoped>
</style>