<template>
  <div class="slider">
    <div class="container">
      <div class="slider-content">
        <h2>Корпоративная жизнь</h2>
        <div class="slider-btn">

          <button class="prevCarusel" @click="prevCarousel">
            <Icon icon="ooui:previous-rtl" color="#a30c33" width="25" height="25" :rotate="2" />
          </button>
          <button class="nextCarusel" @click="nextCarousel">
            <Icon icon="ooui:previous-rtl" color="#a30c33" width="25" height="25" />
          </button>
        </div>
      </div>
      <Carousel ref="carousel" :wrap-around="true" :autoplay="2000" :items-to-show="1">
        <Slide v-for="slide in 1" :key="slide">
          <img src="@/assets/images/slide1.png" alt="">
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="@/assets/images/slide2.png" alt="">
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="@/assets/images/slide3.png" alt="">
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="@/assets/images/slide4.png" alt="">
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="@/assets/images/slide5.png" alt="">
        </Slide>

        <template #addons>
          <Pagination />
        </template>
      </Carousel>
    </div>
  </div>
</template>
<script setup>
import { Icon } from '@iconify/vue';
import { ref } from 'vue';
import { Carousel, Pagination, Slide } from "vue3-carousel";
const carousel = ref()

const nextCarousel = () => carousel.value.next()
const prevCarousel = () => carousel.value.prev()
</script>