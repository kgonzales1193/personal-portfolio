<script lang="ts" setup>
const isClient = ref(false);

onMounted(() => {
  isClient.value = true;
});

const colorMode = useColorMode();
const setColorTheme = () => {
  colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark';
};
</script>

<template>
  <client-only>
    <Button variant="outline" size="icon" class="rounded-full" @click="setColorTheme">
      <IconsMoon v-if="colorMode.value === 'light'" />
      <IconsSun v-else />
    </Button>
  </client-only>
</template>
