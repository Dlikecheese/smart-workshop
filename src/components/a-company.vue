<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow card">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <StarOutlined class="text-blue-500 text-2xl" /><span
            class="text-xl font-bold"
            >企业典型项目</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-8 mb-6">
      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/1.png" alt="" />
        <span class="text-lg">智慧大棚环境监测</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/2.png" alt="" />
        <span class="text-lg">智能家居家电控制</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/3.png" alt="" />
        <span class="text-lg">智慧交通车辆监管</span>
      </div>
    </div>

    <div class="flex justify-between gap-8">
      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/4.png" alt="" />
        <span class="text-lg">智慧仓储货物配送</span>
      </div>

      <div
        class="flex flex-col items-center gap-2 cursor-pointer"
        v-on:click="onClick"
      >
        <img src="@/assets/company/chejian.png" alt="" />
        <span class="text-lg">数字车间集控平台搭建</span>
      </div>

      <div class="flex flex-col items-center gap-2 cursor-pointer">
        <img src="@/assets/company/gongchang.png" alt="" />
        <span class="text-lg">智慧工厂管理平台搭建</span>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import StarOutlined from '@ant-design/icons-vue/StarOutlined'
import { useRouter } from 'vue-router'

const router = useRouter()

const onClick = () => {
  // 用router跳转到详情页，新标签页打开
  const routerData = router.resolve({
    name: 'detail',
    query: { type: 'company' },
  })
  window.open(routerData.href, '_blank')
}
</script>
<style scoped>
@media (min-width: 1455px) {
  img {
    width: 500px;
  }
}

.card {
  background-color: #e6eaf4;
}
</style>
