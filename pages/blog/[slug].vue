<script lang="ts" setup>

const route = useRoute();
console.log(route);
</script>

<template>
  <Bounded>
    Post ID: {{ route.params.slug }}
  </Bounded>
</template>
