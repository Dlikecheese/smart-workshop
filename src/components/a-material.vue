<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow">
    <header class="w-full mb-4">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <FileSearchOutlined class="text-blue-500 text-2xl" /><span
            >工坊数字教材</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>
    </header>

    <div class="flex justify-between gap-4">
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b1.png" alt="" />
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b2.png" alt="" />
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b3.png" alt="" />
      </div>

      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b4.png" alt="" />
      </div>
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b5.png" alt="" />
      </div>
      <div class="flex flex-col items-center gap-2">
        <img src="@/assets/material/b6.png" alt="" />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import FileSearchOutlined from '@ant-design/icons-vue/FileSearchOutlined'
</script>
<style scoped>
@media (max-width: 2500px) {
  img {
    width: 120px;
  }
}

@media (max-width: 1400px) {
  img {
    width: 100px;
  }
}

@media (max-width: 1000px) {
  img {
    width: 80px;
  }
}
</style>
