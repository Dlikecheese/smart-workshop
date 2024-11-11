<template>
  <Header class="w-full header" />
  <Banner />
  <Content />
</template>
<script setup lang="ts">
import Header from '../components/a-header.vue'
import Banner from '../components/a-banner.vue'
import Content from '../components/a-content.vue'
</script>
<style scoped>
.header {
  background-color: #123e93;
}
</style>
