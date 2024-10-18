<template>
  <!-- 虚拟教研介绍 -->
  <div
    class="border-2 border-slate-200 flex m-8 rounded-3xl p-8 shadow items-start gap-4"
  >
    <img src="@/assets/description.png" alt="" class="w-[450px] h-[280px]" />
    <div class="flex flex-col items-center">
      <h2 class="text-xl p-2 font-black">云智工坊介绍</h2>
      <p class="leading-5 mb-6">
        云智工坊是一个多功能的创新和教育平台，它通过提供先进的技术资源和专业化服务，支持教育和创新项目的发展。云智工坊作为创新创业教育的主要阵地，为师生提供了一个低成本、便利化、全要素、开放式的全周期创新创业服务和孵化平台。拥有专兼职创新创业导师团队，提供专业的指导和支持，帮助学生提高创新水平与创业能力。专注于孵化科技企业，对创新成果进行生产转化，帮助学生实现创业梦想。与企业合作，提供真实的产业环境和技术挑战，使学生能够接触并熟悉IT行业企业运营和工作方式。
      </p>
      <a-button type="primary">查看详情 ></a-button>
    </div>
  </div>

  <!-- 教研成员 -->
  <div class="border-2 border-slate-200 m-8 rounded-3xl p-8 shadow">
    <header class="w-full">
      <div class="flex justify-between w-full items-center">
        <div class="flex items-center gap-1 text-xl">
          <TeamOutlined class="text-blue-500" /><span>工坊教师团队</span>
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

  <!-- 企业典型项目 -->
  <a-company />

  <!-- 校企共建资源 -->
  <a-resource />

  <!-- 工坊实景课堂 -->
  <a-course />

  <!-- 工坊数字教材 -->
  <a-material />
</template>
<script setup lang="ts">
import ACompany from '@/components/a-company.vue'
import AResource from '@/components/a-resource.vue'
import ACourse from '@/components/a-course.vue'
import AMaterial from '@/components/a-material.vue'
import { ref } from 'vue'
import { TeamOutlined } from '@ant-design/icons-vue'

const size = ref('small')
import p1 from '@/assets/person/p1.png'
import p2 from '@/assets/person/p2.png'
import p3 from '@/assets/person/p3.png'
import p4 from '@/assets/person/p4.png'
import p5 from '@/assets/person/p5.png'
import p6 from '@/assets/person/p6.png'
import p7 from '@/assets/person/p7.png'
import p8 from '@/assets/person/p8.png'
import router from '@/router'

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
