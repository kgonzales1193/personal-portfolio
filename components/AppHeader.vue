<script lang="ts" setup>


</script>

<template>
  <header class="px-4 md:px-6 py-4 md:py-6 shadow-sm drop-shadow-sm sticky top-0 backdrop-blur-md bg-white/50">
    <div class="container mx-auto">
      <div class="flex flex-col lg:flex-row lg:justify-between items-center gap-2">
        <AppLogo />
        <div class=" lg:inline-flex">
          <nav>
            <ul class="flex gap-6">
              <li>
                <NuxtLink to="/" class="link ">Home
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/about" class="link">
                  About
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/projects" class="link">
                  Projects
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/blog" class="link">
                  Blog
                </NuxtLink>
              </li>
            </ul>
          </nav>
        </div>
        <Button variant="outline" size="icon" class="rounded-full">
          <IconsMoon />
        </Button>
      </div>
    </div>
  </header>
</template>

<style scoped>
.link {
  @apply hover:text-gray-600 text-[18px] font-medium;
}

.router-link-active {
  @apply text-gray-700 pointer-events-none;
}
</style>