<template>
  <section>
    <!-- 虚拟教研介绍 -->
    <a-abstract />

    <div class="mb-8"></div>

    <!-- 教研成员 -->
    <a-member />

    <!-- <img src="@/assets/bg/2.png" alt="" /> -->
  </section>

  <section class="section2">
    <!-- 企业典型项目 -->
    <a-company />

    <div class="mb-8"></div>

    <!-- 校企共建资源 -->
    <a-resource />
  </section>

  <section>
    <!-- 工坊实景课堂 -->
    <a-course />

    <div class="mb-8"></div>

    <!-- 工坊数字教材 -->
    <a-material />
  </section>
</template>
<script setup lang="ts">
import ACompany from '@/components/a-company.vue'
import AResource from '@/components/a-resource.vue'
import ACourse from '@/components/a-course.vue'
import AMaterial from '@/components/a-material.vue'
import AMember from '@/components/a-member.vue'
import AAbstract from '@/components/a-abstract.vue'
</script>
<style scoped>
section {
  padding: 40px 120px;
  background-color: #d9e7fd;
}

@media (min-width: 900px) {
  section {
    padding: 40px 120px;
  }
}

@media (min-width: 1600px) {
  section {
    padding: 40px 200px;
  }
}

@media (min-width: 1900px) {
  section {
    padding: 40px 300px;
    background-color: #d9e7fd;
  }
}

.section2 {
  background-color: #264fa6;
  background-image: url('@/assets/bg/blue.png');
  background-size: cover;
}
</style>
