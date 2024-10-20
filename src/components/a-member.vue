<template>
  <div class="border-2 bg-white border-slate-200 rounded-3xl p-8 shadow">
    <header class="w-full">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-end gap-1 text-xl">
          <TeamOutlined class="text-blue-500 text-2xl" /><span
            class="text-xl font-bold"
            >工坊技术团队</span
          >
        </div>
        <div class="text-blue-500 cursor-pointer">更多 -></div>
      </div>

      <div class="mt-4">
        <a-radio-group
          v-model:value="size"
          style="margin-bottom: 16px"
          button-style="solid"
          @change="onRadioChange"
        >
          <a-radio-button value="company">企业工程师</a-radio-button>
          <a-radio-button value="school">学校双师</a-radio-button>
          <a-radio-button value="student">核心成员</a-radio-button>
        </a-radio-group>
      </div>
    </header>

    <div class="flex px-2 gap-16 flex-wrap">
      <span
        class="flex flex-col justify-center items-center gap-2 avatar-wrap"
        v-for="(member, index) in members"
        :key="index"
      >
        <a-avatar :size="100">
          <template #icon>
            <UserOutlined
              v-if="!member.avatar"
              style="width: 100px !important"
            />
            <img
              v-if="member.avatar"
              :src="member.avatar"
              alt=""
              class="cursor-pointer"
              v-on:click="() => onClick(member)"
            />
          </template>
        </a-avatar>
        <span>{{ member.name }}</span>
      </span>
    </div>
  </div>
</template>
<script setup lang="ts">
import { TeamOutlined, UserOutlined } from '@ant-design/icons-vue'
import { ref } from 'vue'

import p1 from '@/assets/person/p1.png'
import p2 from '@/assets/person/p2.png'
import p3 from '@/assets/person/p3.png'
import p4 from '@/assets/person/p4.png'
import p5 from '@/assets/person/liu.png'
import p6 from '@/assets/person/p5.png'
import huang from '@/assets/person/huangxiujuan.png'
import zhang from '@/assets/person/zhangjun.png'
import cao from '@/assets/person/caokang.png'
import yin from '@/assets/person/yincunju.png'

const size = ref('company')

const members = ref([
  { name: '马万千', avatar: p1 },
  { name: '刘天宋', avatar: p5 },
  { name: '王瑞丽', avatar: p2 },
  { name: '牛宇', avatar: p4 },
])

const onClick = (member: { name: string }) => {
  if (member.name === '刘天宋') {
    window.open(window.location.href + 'detail?type=person')
  }
}

const onRadioChange = (event: { target: { value: string } }) => {
  const value = event.target.value
  if (value === 'company') {
    members.value = [
      { name: '马万千', avatar: p1 },
      { name: '刘天宋', avatar: p5 },
      { name: '王瑞丽', avatar: p2 },
      { name: '牛宇', avatar: p4 },
    ]
  } else if (value === 'school') {
    members.value = [
      { name: '黄秀娟 ', avatar: huang },
      { name: '张俊', avatar: zhang },
      { name: '曹康', avatar: cao },
      { name: '殷存举', avatar: yin },
      { name: '张伟', avatar: p6 },
      { name: '杨天天', avatar: p3 },
    ]
  } else {
    members.value = [
      { name: '王刚', avatar: '' },
      { name: '刘洋', avatar: '' },
      { name: '陈静', avatar: '' },
      { name: '杨磊', avatar: '' },
      { name: '赵敏', avatar: '' },
      { name: '李娜', avatar: '' },
      { name: '张伟', avatar: '' },
      { name: '王丽', avatar: '' },
    ]
  }
}
</script>
<style scoped>
.avatar-wrap :deep(.anticon) {
  position: relative;
  top: -10px;
  font-size: larger;
}
</style>
