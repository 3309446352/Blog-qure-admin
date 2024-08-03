<script lang="ts">
import {defineComponent} from 'vue'
export default defineComponent({
  name: "Window"
})
</script>

<template>
  <div class="flex justify-center items-center h-[560px]">
    <slot>

    </slot>
  </div>
</template>

<style scoped>
div{
  background-color: #f5f7fa;
  border-radius: 4px;
  padding: 20px;
}
</style>