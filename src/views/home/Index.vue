<template>

    <div class="container">
        <div class="list">
            <article-list></article-list>

        </div>
        <div class="cards">

            <el-card class="box-card">
                <div v-for="o in 4" :key="o" class="text item">
                    {{'列表内容 ' + o }}
                </div>
            </el-card>

        </div>

    </div>

</template>

<script lang="ts">
    import {Component, Vue} from "vue-property-decorator";
    import ArticleList from "@/components/article/ArticleList.vue";

    @Component({
        components: {
            ArticleList
        }
    })
    export default class Index extends Vue {
    }
</script>

<style scoped lang="scss">
    .container {
        display: flex;
        flex-direction: row;
        background: #EDEDED;
        height: 100vh;
        padding: 10px;
        .list {
            flex: 1;
        }
        .cards{
             margin-left: 40px;
            flex: 1;
        }
    }
</style>