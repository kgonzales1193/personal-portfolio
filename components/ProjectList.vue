<script lang="ts" setup>
import { Skeleton } from './ui/skeleton';



const { error, pending, data } = await useFetch('https://api.github.com/users/kgonzales1193/repos')

const repos = computed(
  () => (data.value as any[])?.filter(repo => repo.description).sort((a, b) => b.stargazers_count - a.stargazers_count)
)
</script>

<template>
  <Bounded as="section">
    <p class="font-semibold text-lg mb-5">Take a look at my Github projects!</p>
    <div v-if="pending">
      <Skeleton class="w-[100px] h-5 rounded-full" />
    </div>
    <div v-else-if="error">
      <p>Error: {{ error.message }}</p>
    </div>
    <div v-else>
      <ul class="grid grid-cols-1 lg:grid-cols-3 gap-4">
        <li v-for="repo in (repos as any[])" :key="repo.id"
          class="border border-gray-200 rounded-sm p-4 hover:bg-gray-100">
          <a :href="repo.html_url" target="_blank" v-if="data">
            <div class="flex items-center justify-between mb-5">
              <div class="font-semibold">{{ repo.name }}</div>
              <div class="text-gray-500">{{ repo.stargazers_count }}🌟
              </div>
            </div>
            <p class="text-sm text-gray-600">{{ repo.description }}</p>
          </a>
        </li>
      </ul>
    </div>
  </Bounded>
</template>
