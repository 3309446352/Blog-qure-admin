<template>

    <el-slider v-model="size" />
    <el-space wrap :size="size">
      <el-card  v-for="o in 24" style="max-width: 200px;height: 180px">
        <el-icon color="aqua" ><Edit/></el-icon>
        <el-icon color="aqua"><Delete /></el-icon>
        <img src="../assets/GH.jpg" class="image" alt="element" />
      </el-card>
    </el-space>

</template>

<style scoped>

</style>

<script setup lang="ts">
import { Delete, Edit, Search, Share, Upload } from '@element-plus/icons-vue'
definePageMeta(
    { title: '卡片' }
)
const size = ref(7)
</script>
