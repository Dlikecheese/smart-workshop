<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow">
    <header class="w-full">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <TeamOutlined class="text-blue-500 text-2xl" /><span
            >工坊教师团队</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>

      <div class="mt-4">
        <a-radio-group
          v-model:value="size"
          style="margin-bottom: 16px"
          button-style="solid"
        >
          <a-radio-button value="small">企业工程师</a-radio-button>
          <a-radio-button value="default">学校双师</a-radio-button>
          <a-radio-button value="large">优秀小导师</a-radio-button>
        </a-radio-group>
      </div>
    </header>

    <div class="flex justify-between px-2">
      <span
        class="flex flex-col justify-center items-center gap-2"
        v-for="(member, index) in members"
        :key="index"
      >
        <a-avatar :size="100">
          <template #icon>
            <img
              :src="member.avatar"
              alt=""
              class="cursor-pointer"
              v-on:click="onClick"
            />
          </template>
        </a-avatar>
        <span>{{ member.name }}</span>
      </span>
    </div>
  </div>
</template>
<script setup lang="ts">
import { TeamOutlined } from '@ant-design/icons-vue'
import { ref } from 'vue'

import p1 from '@/assets/person/p1.png'
import p2 from '@/assets/person/p2.png'
import p3 from '@/assets/person/p3.png'
import p4 from '@/assets/person/p4.png'
import p5 from '@/assets/person/p5.png'
import p6 from '@/assets/person/p6.png'
import p7 from '@/assets/person/p7.png'
import p8 from '@/assets/person/p8.png'
import router from '@/router'

const size = ref('small')

const members = ref([
  { name: '马万千', avatar: p1 },
  { name: '王瑞丽', avatar: p2 },
  { name: '杨天天', avatar: p3 },
  { name: '牛宇', avatar: p4 },
  { name: '孟杰', avatar: p5 },
  { name: '刘华刚', avatar: p6 },
  { name: '陈道辉', avatar: p7 },
  { name: '朱青松', avatar: p8 },
])

const onClick = () => {
  router.push({ path: '/detail', query: { type: 'person' } })
}
</script>
<style scoped></style>
