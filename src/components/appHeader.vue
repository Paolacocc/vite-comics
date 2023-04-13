<script>
export default {
    name: "appHeader",
    data() {
        return {
            navigationList: [
                {
                    text: "CHARACTES",
                    status: false
                },
                {
                    text: "COMICS",
                    status: true
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
    <div class="header-top">

    </div>
    <div class="container">
    <div class="header">
        <img src="../assets/img/dc-logo.png" alt="">

        <ul class="nav-list">
            <li class="list" v-for="list in navigationList" :class="list.status ? 'active' : ''" ><a href="">{{ list.text }}</a>
            </li>
        </ul>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.header-top {
    height: 30px;
    background-color: black
}

.header {
    @include flex(row, space-between, center);
    
    background-color: white;

    img {
        align-self: flex-start;
        padding: 20px;
    }
    .nav-list {
        margin-left: 30px;
        @include flex(row, center, center);
        .list {
            list-style: none;
            margin-right: 10px;

            a {
                text-decoration: none;
                color: black;
            }
            &.active {

                a {
                    color: $primary-color;
                    border-bottom: 3px solid $primary-color;
                }
               
            }

        }
}
}

</style>