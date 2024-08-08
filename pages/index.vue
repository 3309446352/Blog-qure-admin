<script setup lang="ts">
const staticsData = ref({
  articleCount: 0,
  categoryCount: 0,
  tagCount: 0,
  userCount: 0,
  commitList: []
});
import HomeCard from "@/components/HomeCard/home-card.vue";
</script>

<template>
  <el-card class="home">
    <template #header> 首页 </template>
    <el-row>
      <el-col :xs="12" :sm="6">
        <home-card label="文章" :value="staticsData.articleCount">
          <img src="@/assets/svg/biaoqian.svg" alt="" class="w-[48px] h-[48px] svg-fill">
        </home-card>
      </el-col>
      <el-col :xs="12" :sm="6">
        <home-card label="分类" :value="staticsData.categoryCount">
          <img src="@/assets/svg/fenlei.svg" alt="" class="w-[48px] h-[48px] svg-fill" />
        </home-card>
      </el-col>
      <el-col :xs="12" :sm="6">
        <home-card label="标签" :value="staticsData.tagCount">
          <img src="@/assets/svg/biaoqian.svg" alt="" class="w-[48px] h-[48px] svg-fill" />
        </home-card>
      </el-col>
      <el-col :xs="12" :sm="6">
        <home-card label="用户" :value="staticsData.userCount">
          <img src="@/assets/svg/yonghu.svg" class="w-[48px] h-[48px] svg-fill" />
        </home-card>
      </el-col>
    </el-row>
    <el-row class="mt-4">
      <el-col :sm="24" :xs="0">
        <h1>最新评论</h1>
      </el-col>
    </el-row>
    <el-row>
      <el-col :xs="24" :sm="12">
        <el-card class="m-[5px]">

        </el-card>
      </el-col>
      <el-col :xs="24" :sm="12">
        <el-card class="m-[5px]">

        </el-card>
      </el-col>
    </el-row>
  </el-card>
</template>

<style scoped>
h1{
  font: 400 40px/1.5 'Bree Serif', 'Lora', 'Playfair Display', Georgia, serif;
}
</style>