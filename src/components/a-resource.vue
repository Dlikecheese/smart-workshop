<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow card">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <MergeCellsOutlined class="text-blue-500 text-2xl" /><span
            class="text-xl font-bold"
            >校企共建资源库</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-2">
      <a
        class="flex flex-col items-center gap-2 cursor-pointer"
        href="https://czlgj.fy.chaoxing.com/portal/"
        target="_blank"
      >
        <img src="@/assets/resource/1.png" alt="" />
        <span>教学云</span>
      </a>

      <a
        class="flex flex-col items-center gap-2 cursor-pointer"
        href="http://124.221.240.160:8891/"
        target="_blank"
      >
        <img src="@/assets/resource/2.png" alt="" />
        <span>企业云</span>
      </a>

      <a
        class="flex flex-col items-center gap-2 cursor-pointer"
        href="http://101.35.221.158:8000/SysModules/Login/Login.aspx"
        target="_blank"
      >
        <img src="@/assets/resource/3.png" alt="" />
        <span>工业云</span>
      </a>

      <a
        class="flex flex-col items-center gap-2 cursor-pointer"
        href="https://wuqiyang312.github.io/ai-pages/"
        target="_blank"
      >
        <img src="@/assets/resource/4.png" alt="" />
        <span>工具云</span>
      </a>
    </div>
  </div>
</template>
<script setup lang="ts">
import MergeCellsOutlined from '@ant-design/icons-vue/MergeCellsOutlined'
</script>
<style scoped>
.card {
  background-color: #e6eaf4;
}
</style>
