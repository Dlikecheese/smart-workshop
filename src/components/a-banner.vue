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
    <img src="@/assets/banner/A1.jpg" alt="" />
    <img src="@/assets/banner/A2.jpg" alt="" />
    <img src="@/assets/banner/A3.jpg" alt="" />
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
</style>
