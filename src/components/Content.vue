<template>
  <!-- 虚拟教研介绍 -->
  <div
    class="border-2 border-slate-200 flex m-8 rounded-3xl p-8 shadow items-start gap-4"
  >
    <img src="@/assets/description.png" alt="" class="w-[450px] h-[280px]" />
    <div class="flex flex-col items-center">
      <h2 class="text-xl p-2 font-black">云智工坊介绍</h2>
      <p class="leading-5 mb-6">
        云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍云智工坊介绍介绍云智工坊介绍云智工坊介绍介绍云智工坊介绍云智工坊介绍介绍云智工坊介绍云智工坊介绍介绍云智工坊介绍云智工坊介绍介绍云智
      </p>
      <a-button type="primary">查看详情 ></a-button>
    </div>
  </div>

  <!-- 教研成员 -->
  <div class="border-2 border-slate-200 flex m-8 rounded-3xl p-8 shadow">
    <header class="flex justify-between w-full">
      <div class="flex items-center gap-1 text-xl">
        <TeamOutlined class="text-blue-500" /><span>教研成员</span>
      </div>
      <div class="text-blue-500">更多 -></div>
    </header>
    <div></div>
  </div>
</template>
<script setup lang="ts">
import { TeamOutlined } from '@ant-design/icons-vue'
</script>
<style scoped></style>
