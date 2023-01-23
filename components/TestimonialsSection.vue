<script setup>
import { ButtonTypes } from '~/server/api/types'
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Navigation, Pagination, Slide } from 'vue3-carousel'

const testimonials = [
  {
    title: 'Lorem 1',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.',
    btnText: 'Leer más',
    img: '/_nuxt/assets/dogs8.jpg',
  },
  {
    title: 'Lorem 2',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.',
    btnText: 'Leer más',
    img: '/_nuxt/assets/dogs9.jpg',
  },
  {
    title: 'Lorem 3',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.',
    btnText: 'Leer más',
    img: '/_nuxt/assets/dogs10.jpg',
  },
  {
    title: 'Lorem 4',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.',
    btnText: 'Leer más',
    img: '/_nuxt/assets/dogs11.jpg',
  },
  {
    title: 'Lorem 5',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.',
    btnText: 'Leer más',
    img: '/_nuxt/assets/dogs12.jpg',
  },
]
</script>

<template>
  <div py-8 bg-gray-2>
    <p class="font-tous tracking-widest text-xs">
      Lorem ipsum
    </p>
    <h1 class="font-tous text-[34px]">
      Lorem ipsum
    </h1>
    <p text-xs py-4>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt.
    </p>
    <CtaBtn
      label="CTA 3"
      :type="ButtonTypes.tertiary"
      class="mb-4"
    />

    <Carousel hidden md:block :items-to-show="3">
      <Slide v-for="(item, index) in testimonials" :key="index">
        <div px-2>
          <Testimonial :title="item.title" :description="item.description" :btn-text="item.btnText" :img="item.img" />
        </div>
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>

    <Carousel md:hidden :items-to-show="1.2">
      <Slide v-for="(item, index) in testimonials" :key="index">
        <div px-2>
          <Testimonial :title="item.title" :description="item.description" :btn-text="item.btnText" :img="item.img" />
        </div>
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>
  </div>
</template>

<style scoped>

</style>
