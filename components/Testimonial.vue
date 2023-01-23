<script setup>
import { ButtonTypes } from '~/server/api/types'

const props = defineProps({
  title: String,
  description: String,
  btnText: String,
  img: String,
})
</script>

<template>
  <div row-span-1>
    <img :src="props.img" :alt="props.title" class="aspect-square object-cover">
    <h1 class="font-tous text-[34px]">
      {{ props.title }}
    </h1>
    <p text-xs py-4>
      {{ props.description }}
    </p>
    <CtaBtn
      :label="props.btnText" :type="ButtonTypes.tertiary"
    />
  </div>
</template>
