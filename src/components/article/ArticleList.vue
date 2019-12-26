<template>
    <div>

        <el-table
                :data="tableData"
                :show-header="false"
                style="width: 100%">
            <el-table-column
                    prop="date"
                    width="180">
            </el-table-column>
            <el-table-column
                    prop="name"
                    width="180">
            </el-table-column>
            <el-table-column
                    prop="address"
                    >
            </el-table-column>
        </el-table>
        <el-pagination
                background
                layout="prev, pager, next"
                :total="1000">
        </el-pagination>
    </div>

</template>

<script lang="ts">

    import {Component, Vue} from "vue-property-decorator";

    @Component
    export default class ArticleList extends Vue {
        tableData: any = [ {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
        }  ]
    }
</script>

<style>

</style>