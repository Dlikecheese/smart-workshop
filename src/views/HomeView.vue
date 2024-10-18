<template>
  <Header class="absolute z-20 w-full" />
  <Banner />
  <div class="m-20">
    <Content />
  </div>
</template>
<script setup lang="ts">
import Header from '../components/Header.vue'
import Banner from '../components/Banner.vue'
import Content from '../components/Content.vue'
</script>
<style scoped></style>
