<template>

    <div>

        <div class="page-warpper">

            <div class="logo">
                <img src="https://www.oudahe.com/themes/default/styles/images/logo.png" alt="" style="margin-top: 20px">
            </div>
            <ol class="nav">
                <li @click="handleClick" v-for="item in list"><span>{{item}}</span></li>

            </ol>


        </div>


    </div>

</template>

<script lang="ts">
    import {Component, Vue} from "vue-property-decorator";

    export default class Home extends Vue {
        list: Array<string> = ['这是一个什么啊', '这是一个什么啊', '这是一个什么啊', '这是一个什么啊', '这是一个什么啊']

        handleClick(): void {
            alert(22)
        }
    }
</script>

<style lang="scss" scoped>

    .page-warpper {
        background: #323841;
        height: 100vh;
        .logo {
            width: 100px;
            height: 100px;
            font-size: 0;

        }

        .nav {
            padding: 0px 20px;

            li {
                padding: 13px;
                color: #ddd;

                &:hover {
                    background: #8463a9;
                    color: #f8f8f8;
                }

                &.active {
                    background: #09b1b9;
                    color: #f8f8f8;
                }

            }

        }
    }


</style>