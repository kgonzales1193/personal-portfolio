<template>
  <div id="viewport">
    <AppHeader />
    <main>
      <slot />
      <div class="h-screen"></div>
    </main>
    <AppFooter />
  </div>
</template>

<script lang="ts" setup>

useHead({
  htmlAttrs: {
    lang: 'en'
  },
  link: [
    {
      rel: 'icon',
      type: 'image/png',
      href: '/favicon.ico'
    }
  ]
})

</script>
