<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <VideoCameraTwoTone class="text-blue-500 text-2xl" /><span
            class="text-xl font-bold"
            >工坊实景课堂</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-2 mb-4">
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/course/1.png" alt="" />
        <span>农业大棚</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/course/2.png" alt="" />
        <span>家居家电</span>
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/course/3.png" alt="" />
        <span>交通车辆</span>
      </div>
    </div>

    <div class="flex justify-between gap-2">
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/course/4.png" alt="" />
        <span>仓储货物</span>
      </div>

      <a
        class="flex flex-col items-center gap-2 cursor-pointer"
        href="https://www.720yun.com/vr/a93jzswOuO1"
        target="_blank"
      >
        <img src="@/assets/course/5.png" alt="" />
        <span>数字车间</span>
      </a>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/course/6.png" alt="" />
        <span>智慧工厂</span>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import VideoCameraTwoTone from '@ant-design/icons-vue/VideoCameraTwoTone'
</script>
<style scoped>
@media (min-width: 1455px) {
  img {
    width: 500px;
  }
}
</style>
