<template>
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8 pb-12">
    <a name="contact"></a><h2 class="text-2xl font-bold text-white">Contact</h2>
    <ul role="list" class="divide-y divide-gray-800">
      <li v-for="way in ways" :key="way.email" class="flex justify-between gap-x-6 py-5">
        <div class="flex min-w-0 gap-x-4">
          <img class="size-12 flex-none rounded-full bg-gray-50" :src="way.imageUrl" alt="" />
          <div class="min-w-0 flex-auto">
            <p class="text-sm/6 font-semibold text-white">{{ way.name }}</p>
            <p class="mt-1 truncate text-sm/5 text-gray-400"><a :href="`mailto:${way.email}`">{{ way.email }}</a></p>
          </div>
        </div>
        <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
          <p class="text-xs/6 text-white">{{ way.domain }}</p>
          <div v-if="way.isMain" class="mt-1 flex items-center gap-x-1.5">
            <div class="flex-none rounded-full bg-emerald-500/20 p-1">
              <div class="size-1.5 rounded-full bg-emerald-500" />
            </div>
            <p class="text-xs/5 text-gray-400">Mainly used</p>
          </div>
          <p v-else class="mt-1 text-xs/5 text-gray-400">
            Occasionally used
          </p>
        </div>
      </li>
    </ul>
  </div>
</template>
  
<script setup lang="ts">
const ways = [
  {
    name: 'Personal Email',
    email: 'tomhwi01@gmail.com',
    domain: 'Gmail',
    imageUrl:
      'https://workspace.google.com/static/favicon.ico',
    isMain: true,
  },
  {
    name: 'Personal Email',
    email: 'tomhwi01@outlook.com',
    domain: 'Mcrosoft Outlook',
    imageUrl:
      'https://cdn-dynmedia-1.microsoft.com/is/content/microsoftcorp/Icon-Outlook-28x281?resMode=sharp2&amp;op_usm=1.5,0.65,15,0&amp;qlt=85',
    isMain: false,
  },
]
</script>