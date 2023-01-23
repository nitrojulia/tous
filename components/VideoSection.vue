<script setup>
import { ButtonTypes } from '~/server/api/types'
</script>

<template>
  <div flex justify-around class="flex-wrap-reverse md:flex-wrap pb-[10%] pt-[10%] md:pt-0">
    <div class="pb-[5%]">
      <p class="py-[5%] md:px-[10%] px-[5%]">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt. Donec placerat gravida imperdiet. Sed gravida pretium pulvinar. Duis porttitor dolor rhoncus, tempus enim id, lacinia elit. Aliquam posuere felis in placerat luctus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nunc in lorem euismod, dictum mi in, commodo orci.
      </p>
      <div class="bg w-full min-h-[400px] absolute -z-1 filter-blur-[3px] hidden md:block" />
    </div>
    <div class="w-full md:w-auto flex justify-center md:px-0 px-[5%]">
      <img src="/dogs1.jpg" alt="dog1" class="w-[400px]">
    </div>
    <div flex flex-col text-left class="md:text-white pb-[10%] md:px-0 px-[5%]">
      <p text="xs">
        Lorem ipsum
      </p>
      <h1 class="font-tous text-[34px]">
        Lorem ipsum
      </h1>
      <p class="md:max-w-[40vw] text-sm py-2">
        Lorem ipsum <br>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a mi fringilla nisi condimentum tincidunt. Donec placerat gravida imperdiet. Sed gravida pretium pulvinar. Duis porttitor dolor rhoncus, tempus enim id, lacinia elit. Aliquam posuere felis in placerat luctus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nunc in lorem euismod, dictum mi in, commodo orci.
      </p>
      <CtaBtn label="CTA 1" class="mb-2" />
      <CtaBtn label="CTA 2" :type="ButtonTypes.secondary" />
    </div>
  </div>
</template>

<style scoped>
.bg{
  background-image: url("/dogs4.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
</style>
