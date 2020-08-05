<template>
  <div class="top-view">
    <el-row :gutter="20">
      <el-col :span="6">
        <el-card shadow="hover" :body-style="{padding:20}">
          <total-sales />
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-orders />
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <today-users />
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-users />
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import TotalSales from "./../TotalSales/index";
import TotalOrders from './../TotalOrders/index';
import TotalUsers from './../TotalUsers/index';
import TodayUsers from './../TodayUsers/index'
export default {
  components: {
    TotalSales,
    TotalOrders,
    TotalUsers,
    TodayUsers
  },
};
</script>

<style>
</style>
