<template>
  <div flex flex-col justify-center items-center colum class="carousel-main md:py-[10%] pt-[25%] pb-[5%]">
    <h1>Lorem Ipsum</h1>
    <h3>Lorem ipsum dolor sit amet</h3>
  </div>
</template>

<style scoped>
.carousel-main {
  background-image: url("assets/dogs7.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
.carousel-main h1, .carousel-main h3 {
  color: white;
  text-shadow: #333 3px 3px 10px;
}
h1 {
  font-family: Tous, Tous-fallback;
  font-weight: 600;
  font-size: 34px;
}
h3 {
  font-family: Roboto, Roboto-fallback;
  font-size: 16px;
}
</style>
