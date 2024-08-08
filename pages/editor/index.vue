

<template>
  <el-card shadow="never">
    <el-collapse  accordion >
      <MdEditor v-model="text" :theme="theme"/>

    </el-collapse>
  </el-card>
</template>

<style lang="scss" scoped>
:deep(.el-collapse-item__header) {
  padding-left: 10px;
}
</style>
<script setup lang="ts">
import { ref } from "vue";
// import  EditorBase from "./components/EditorBase.vue";
// import   EditorMulti from "./components/EditorMulti.vue";
// import  EditorUpload from "./components/EditorUpload.vue";
defineOptions({
  name: "Editor"
});
definePageMeta(
    { title: '编辑器' }
)
import { MdEditor } from 'md-editor-v3';
import 'md-editor-v3/lib/style.css';

const text = ref('# Hello Editor');
const theme = ref('light');
</script>