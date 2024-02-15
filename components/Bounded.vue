<script lang="ts" setup>
defineProps<{
  as?: string;
}>();
</script>

<template>
  <Component :is="as || 'section'" class="px-4 md:px-6 py-4 md:py-10 lg:py-14">
    <div class="max-w-[1280px] container mx-auto">
      <slot />
    </div>
  </Component>
</template>
