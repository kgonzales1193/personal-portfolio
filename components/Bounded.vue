<script lang="ts" setup>
defineProps<{
  as?: string;
}>();
</script>

<template>
  <Component :is="as || 'section'" class="px-4 md:px-6 py-10 md:py-14 lg:py-16">
    <div class="container mx-auto">
      <slot />
    </div>
  </Component>
</template>
