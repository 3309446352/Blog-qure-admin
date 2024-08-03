<template>
    <Window>
      <el-card style="max-width: 100%" v-for="o in 4">
        <p v-for="o in 4" :key="o" class="text item">{{ 'List item ' + o }}</p>
      </el-card>
    </Window>
</template>

<style scoped>

</style>

<script setup lang="ts">

</script>
