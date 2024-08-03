<template>
  <div class="common-layout">
    <el-container>
      <el-aside width="200px"><CollapseMenu/></el-aside>
      <el-container>
        <el-header>
          <Breadcrumb/>
        </el-header>
        <el-main>
          <Window>
            <slot />
          </Window>
        </el-main>
        <el-footer>
          <h2> 版权所有 © 2020-present PureAdmin</h2>
        </el-footer>
      </el-container>
    </el-container>
  </div>
</template>
<style>
h2{
  text-align: center;
  color: #999;
  font-size: 14px;
}
</style>

<script setup lang="ts">
import Breadcrumb from "~/components/Breadcrumb.vue";
import CollapseMenu from "~/components/Collapse-menu.vue";
</script>
