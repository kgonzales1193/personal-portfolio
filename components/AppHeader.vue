<script lang="ts" setup>


</script>

<template>
  <header class="px-4 md:px-6 py-4 md:py-6 border-b sticky top-0 backdrop-blur-md">
    <div class="max-w-[1280px] container mx-auto">
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
        <ThemeToggle />
      </div>
    </div>
  </header>
</template>

<style scoped>
.link {
  @apply hover:text-gray-600 text-[18px] font-medium;
}

.router-link-active {
  @apply text-gray-600 dark:text-gray-400 pointer-events-none;
}
</style>