<template>
  <a-carousel arrows autoplay>
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
      <div class="text-wrap">
        <span class="mr-4 text">云智启航</span>
        <span class="mr-10 text">工坊筑梦</span>
      </div>
    </div>
    <div class="img img2">
      <span class="inline-block">
        <span class="mr-4 text">云智工坊</span>
        <span class="text">引领未来</span></span
      >
    </div>
    <div class="img img3">
      <span class="inline-block text-wrap">
        <span class="mr-4 text">产教联合</span>
        <span class="text">共育新才</span>
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
  /* height: 250px; */
  width: 100%;
  text-align: center;
  font-size: 30px;
  color: #fff;
  background-size: cover;
  background-position: center;
}
.text {
  font-family: 'YouSheTitleBlack', sans-serif;
  font-size: 50px;
  letter-spacing: 6px;
  line-height: 250px;
}

.text-wrap {
  margin-left: 65%;
}

.img1 {
  background-image: url(@/assets/banner/1.png);
}

.img2 {
  background-image: url(@/assets/banner/2.png);
  line-height: 250px;
  padding-left: 100px;
  text-align: start;
}

.img3 {
  background-image: url(@/assets/banner/3.png);
  text-align: end;
  padding-right: 100px;
}
</style>
