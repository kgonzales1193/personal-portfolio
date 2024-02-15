<template>
  <div>
    <div class="container mx-auto py-10">
      <nav>
        <ul class="flex items-center justify-center gap-5">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/blog">Blog</NuxtLink>
          </li>
        </ul>
      </nav>
    </div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
