<template>
  <a-carousel arrows>
    <template #prevArrow>
      <div class="custom-slick-arrow" style="left: 10px; z-index: 1">
        <left-circle-outlined />
      </div>
    </template>
    <template #nextArrow>
      <div class="custom-slick-arrow" style="right: 10px">
        <right-circle-outlined />
      </div>
    </template>
    <div class="img img1">
      <span class="mr-4">云智启航</span> <span class="mr-10">工坊筑梦</span>
    </div>
    <div class="img img2">
      <span class="inline-block">
        <span class="mr-4">云智工坊</span> <span>引领未来</span></span
      >
    </div>
    <div class="img img3">
      <span class="inline-block">
        <span class="mr-4">产教联合</span> <span>共育新才</span>
      </span>
    </div>
  </a-carousel>
</template>
<script setup lang="ts">
import { LeftCircleOutlined, RightCircleOutlined } from '@ant-design/icons-vue'
</script>
<style scoped>
.ant-carousel :deep(.slick-slide) {
  text-align: center;
  /* height: 160px; */
  line-height: 160px;
  background: #364d79;
  overflow: hidden;
}

.ant-carousel :deep(.slick-arrow.custom-slick-arrow) {
  width: 25px;
  height: 25px;
  font-size: 25px;
  color: #fff;
  background-color: rgba(31, 45, 61, 0.11);
  opacity: 0.3;
}
.ant-carousel :deep(.custom-slick-arrow:before) {
  display: none;
}
.ant-carousel :deep(.custom-slick-arrow:hover) {
  opacity: 0.5;
}

.ant-carousel :deep(.slick-slide h3) {
  color: #fff;
}

.img {
  height: 250px;
  width: 100%;
  text-align: center;
  font-size: 30px;
  color: #fff;
  line-height: 250px;
  letter-spacing: 10px;
  font-weight: 800;
}

.img1 {
  background-image: url(@/assets/banner/1.png);
  background-size: cover;
  background-position: 100% 100%;
  text-align: end;
}

.img2 {
  background-image: url(@/assets/banner/2.png);
  background-size: cover;
  background-position: 100% 100%;
  line-height: 250px;
  padding-left: 100px;
  text-align: start;
}

.img3 {
  background-image: url(@/assets/banner/3.png);
  background-size: cover;
  background-position: 100% 100%;
  text-align: end;
  padding-right: 100px;
}
</style>
