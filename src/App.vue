<template>
    <div id="app">
        <el-container>
            <el-aside width="200px">  <Home></Home></el-aside>
            <el-container>
                <el-header class="header">Header</el-header>
                <el-main><router-view></router-view></el-main>
            </el-container>
        </el-container>
    </div>
</template>
<script lang="ts">

    import {Component, Vue} from "vue-property-decorator";
    import Home from "@/views/home/Home.vue";

    @Component({
        components: {
            Home,
        }
    })
    export default class App extends Vue {

    }


</script>
<style lang="scss">

    * {
        padding: 0;
        margin: 0;
        border: 0;
        overflow: hidden;

    }

    a {
        text-decoration: none;
        color: inherit;
    }

    li {
        list-style: none;
    }

    #app {
        display: flex;
        flex-direction: row;


    }



    .el-header {
        background: #323841;
        text-align: center;
    }
    .el-main{
        padding: 0 !important;
    }

</style>
