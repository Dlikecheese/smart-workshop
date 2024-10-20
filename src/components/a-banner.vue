<template>
  <a-carousel arrows autoplay="true">
    <template #prevArrow>
      <div class="custom-slick-arrow" style="left: 10px; zindex: 1">
        <left-circle-outlined />
      </div>
    </template>
    <template #nextArrow>
      <div class="custom-slick-arrow" style="right: 10px">
        <right-circle-outlined />
      </div>
    </template>
    <div><img src="@/assets/banner/b1.png" class="w-full" /></div>
    <div><img src="@/assets/banner/b2.png" class="w-full" /></div>
    <div><img src="@/assets/banner/b3.png" class="w-full" /></div>
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

@media (max-width: 1740px) {
  img {
    height: 500px;
  }
}

@media (max-width: 1440px) {
  img {
    height: 450px;
  }
}

@media (max-width: 800px) {
  img {
    height: 250px;
  }
}
</style>
