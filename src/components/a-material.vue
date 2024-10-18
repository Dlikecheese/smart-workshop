<template>
  <div class="border-2 border-slate-200 m-8 rounded-3xl p-8 shadow">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-center gap-1 text-xl">
          <FileSearchOutlined class="text-blue-500" /><span>工坊数字教材</span>
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-2">
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/1.png" alt="" />
        <span>智慧大棚环境监测</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/2.png" alt="" />
        <span>智能家居家电控制</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/3.png" alt="" />
        <span>智慧交通车辆监管</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/4.png" alt="" />
        <span>智慧仓储货物配送</span>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import FileSearchOutlined from '@ant-design/icons-vue/FileSearchOutlined'
</script>
<style scoped>
img {
  width: 300px;
  height: 170px;
}
</style>
