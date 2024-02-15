<template>
  <Bounded as="section">
    <div class="max-w-4xl mx-auto flex flex-col items-center justify-center">
      <h1 class="text-4xl font-bold">Welcome to My Portfolio</h1>
      <p class="text-lg mt-4">This is a simple portfolio website built with VitePress</p>
    </div>
  </Bounded>
</template>

<script lang="ts" setup>
useSeoMeta({
  title: 'iDev\'s Portfolio - Home',
  description: 'Portfolio website built with Nuxt',
  ogTitle: 'iDev\'s Portfolio',
  ogDescription: 'Portfolio website built with Nuxt',
  ogImage: '/codethinking.svg',
  ogUrl: '/codethinking.svg',
  twitterTitle: 'iDev\'s Portfolio',
  twitterDescription: 'Portfolio website built with Nuxt',
  twitterImage: '/codethinking.svg',
  twitterCard: 'summary_large_image'
})

</script>

