<template>
  <Bounded>
    <div class="text-center">
      <h2 class="text-3xl lg:text-6xl font-bold">Projects</h2>
    </div>
    <ProjectList />
  </Bounded>
</template>

<script lang="ts" setup>
useSeoMeta({
  title: 'iDev\'s Portfolio - Projects',
  description: 'My projects and works.',
  ogTitle: 'iDev\'s Portfolio',
  ogDescription: 'My projects and works.',
  ogImage: '/codethinking.svg',
  ogUrl: '/codethinking.svg',
  twitterTitle: 'iDev\'s Portfolio',
  twitterDescription: 'My projects and works.',
  twitterImage: '/codethinking.svg',
  twitterCard: 'summary_large_image'
})
</script>

<style></style>