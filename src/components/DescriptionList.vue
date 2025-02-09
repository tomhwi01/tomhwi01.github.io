<template>
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
    <a name="about-me"><h2 class="text-2xl font-bold text-white">About me</h2></a>
    <div class="px-4 sm:px-0">
      <p class="mt-1 max-w-2xl text-sm/6 text-gray-400">Personal details and skills.</p>
    </div>
    <div class="mt-6 border-t border-gray-800">
      <dl class="divide-y divide-gray-800">
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Name</dt>
          <dd class="mt-1 text-sm/6 text-gray-400 sm:col-span-2 sm:mt-0">Tom Ho</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Gender</dt>
          <dd class="mt-1 text-sm/6 text-gray-400 sm:col-span-2 sm:mt-0">Male</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Location</dt>
          <dd class="mt-1 text-sm/6 text-gray-400 sm:col-span-2 sm:mt-0">Hong Kong</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Languages</dt>
          <dd class="mt-1 text-sm/6 text-gray-400 sm:col-span-2 sm:mt-0">Chinese - Cantonese: &nbsp;&nbsp;Native<br />Chinese - Mandarin: &nbsp;&nbsp;Fluent<br />English: &nbsp;&nbsp;Conversational</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Education</dt>
          <dd class="mt-1 text-sm/6 text-gray-400 sm:col-span-2 sm:mt-0">Bachelor of Engineering (Information Engineering) - Upper Second Class Honours, City University of Hong Kong</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm/6 font-medium text-white">Skills</dt>
          <dd class="mt-2 text-sm text-white sm:col-span-2 sm:mt-0">
            <ul role="list" class="divide-y divide-gray-800 rounded-md border border-gray-700">
              <li class="flex items-center justify-between py-4 pr-5 pl-4 text-sm/6">
                <div class="flex w-0 flex-1 items-center">
                  <img src="https://www.python.org/static/favicon.ico" class="h-6" alt="Python logo" />
                  <div class="ml-4 flex min-w-0 flex-1 gap-2">
                    <span class="shrink-1 font-medium">Python</span>
                    <span class="truncate text-gray-400">tensorflow, keras, fastapi, mariadb, etc.</span>
                  </div>
                </div>
                <div class="ml-4 shrink-1">
                  <a href="https://www.python.org/" target="_blank" rel="noopener noreferrer" class="font-medium text-blue-400 hover:text-blue-500">Official Website</a>
                </div>
              </li>
              <li class="flex items-center justify-between py-4 pr-5 pl-4 text-sm/6">
                <div class="flex w-0 flex-1 items-center">
                  <div class="ml-4 flex min-w-0 flex-1 gap-2">
                    <span class="shrink-1 font-medium">Java, Android Studio, C#, Arduino C, Matlab, SAS, HTML, Vue.js, Tailwind CSS</span>
                    <span class="shrink-0 text-gray-400">brief understanding</span>
                  </div>
                </div>
              </li>
            </ul>
          </dd>
        </div>
      </dl>
    </div>
  </div>
</template>
  
<script setup lang="ts">
</script>