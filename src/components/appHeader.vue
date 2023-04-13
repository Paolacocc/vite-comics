<script>
export default {
    name: "appHeader",
    data(){
        return{
            navigationList: [
                {
                text: "CHARACTES",
                status: false
            },
            {
                text: "COMICS",
                status: false
            },
            {
                text: "MOVIES",
                status: false
            },
            {
                text: "TV",
                status: false
            },
            {
                text: "GAMES",
                status: false
            },
            {
                text: "COLLECTABLES",
                status: false
            },
            {
                text: "VIDEO",
                status: false
            }, 
            {
                text: "FANS",
                status: false
            },
            {
                text: "NEWS",
                status: false
            }
        ]
        }
    }
    

}
</script>

<template>
    <img src="../assets/img/dc-logo.png" alt="">

    <ul class="nav-list">
        <li class="list" v-for="list in navigationList"><a href="">{{ list.text }}</a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
.nav-list {
 .list {
    text-decoration: none;
 }
}
</style>