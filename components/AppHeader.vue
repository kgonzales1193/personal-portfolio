<script lang="ts" setup>

const route = useRoute()
console.log(route);

const isActive = (path: string) => route.path === path;

</script>

<template>
  <header class="px-4 md:px-6 py-4 md:py-6 lg:py-8">
    <div class="container mx-auto">
      <div class="flex justify-between items-center">
        <a href="/" class="text-2xl font-bold">iDev&apos;s Portfolio</a>
        <div class="hidden lg:inline-flex">
          <nav>
            <ul class="flex font-medium gap-6 ">
              <li>
                <NuxtLink to="/" class="hover:text-gray-600"
                  :class="{ 'text-gray-700 pointer-events-none': isActive('/') }">Home</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/about" class="hover:text-gray-600"
                  :class="{ 'text-gray-700 pointer-events-none': isActive('/about') }">About</NuxtLink>
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
