<template>
  <Suspense>
    <main>
      <CarouselMain />
      <VideoSection />
      <GallerySection />
      <TestimonialsSection />
    </main>
    <template #fallback>
      <div op50 italic>
        <span animate-pulse>Loading...</span>
      </div>
    </template>
  </Suspense>
</template>
