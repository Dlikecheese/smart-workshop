<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <MergeCellsOutlined class="text-blue-500 text-2xl" /><span
            >校企共建资源库</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-2">
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/resource/1.png" alt="" />
        <span>教学云</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/resource/2.png" alt="" />
        <span>企业云</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/resource/3.png" alt="" />
        <span>工业云</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/resource/4.png" alt="" />
        <span>工具云</span>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import MergeCellsOutlined from '@ant-design/icons-vue/MergeCellsOutlined'
</script>
<style scoped></style>
