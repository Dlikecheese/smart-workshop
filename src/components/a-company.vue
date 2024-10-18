<template>
  <div class="border-2 border-slate-200 m-8 rounded-3xl p-8 shadow">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-center gap-1 text-xl">
          <StarOutlined class="text-blue-500" /><span>企业典型项目</span>
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-2">
      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/1.png" alt="" />
        <span>智慧大棚环境监测</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/2.png" alt="" />
        <span>智能家居家电控制</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/3.png" alt="" />
        <span>智慧交通车辆监管</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/4.png" alt="" />
        <span>智慧仓储货物配送</span>
      </div>

      <div
        class="flex flex-col items-center gap-2 cursor-pointer"
        v-on:click="onClick"
      >
        <img src="@/assets/company/5.png" alt="" />
        <span>数字车间集控平台搭建</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/6.png" alt="" />
        <span>智慧工厂综合管理系统搭建</span>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import router from '@/router'
import StarOutlined from '@ant-design/icons-vue/StarOutlined'

const onClick = () => {
  router.push({ path: '/detail', query: { type: 'company' } })
}
</script>
<style scoped></style>
