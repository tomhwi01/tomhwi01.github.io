<template>
  <div class="absolute inset-x-0 -top-40 transform-gpu overflow-hidden blur-3xl sm:-top-80" aria-hidden="true">
    <div class="relative left-[calc(50%-11rem)] aspect-1155/678 w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-linear-to-tr from-[#80caff] to-[#4f46e5] opacity-30 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)" />
  </div>
  <div class="absolute inset-x-0 bottom-0 transform-gpu overflow-hidden blur-3xl" aria-hidden="true">
    <div class="relative left-[calc(50%+3rem)] aspect-1155/678 w-[36.125rem] -translate-x-1/2 bg-linear-to-tr from-[#80caff] to-[#4f46e5] opacity-30 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)" />
  </div>
  <div class="flex items-center isolate px-6 pt-14 lg:px-8 min-h-screen">
    <header class="absolute inset-x-0 top-0 z-50">
      <nav class="p-6 lg:px-8" aria-label="Global">
        <div class="text-end lg:hidden">
          <div class="inline">
            <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = true">
              <span class="sr-only">Open main menu</span>
              <svg xmlns="http://www.w3.org/2000/svg" xml:space="preserve" class="text-gray-400 fill-current h-6" alt="Menu button" viewBox="0 0 250.579 250.579"><path d="M22.373 76.068h205.832c12.356 0 22.374-10.017 22.374-22.373 0-12.356-10.017-22.373-22.374-22.373H22.373C10.017 31.323 0 41.339 0 53.696c0 12.356 10.017 22.372 22.373 22.372zm205.832 26.848H22.373C10.017 102.916 0 112.933 0 125.289c0 12.357 10.017 22.373 22.373 22.373h205.832c12.356 0 22.374-10.016 22.374-22.373 0-12.356-10.018-22.373-22.374-22.373zm0 71.594H22.373C10.017 174.51 0 184.526 0 196.883c0 12.356 10.017 22.373 22.373 22.373h205.832c12.356 0 22.374-10.017 22.374-22.373 0-12.357-10.018-22.373-22.374-22.373z" style="fill-rule:evenodd;clip-rule:evenodd"/></svg>
            </button>
          </div>
        </div>
        <div class="text-center hidden lg:block">
          <div class="lg:inline-flex lg:gap-x-12">
            <a v-for="item in navigation" :key="item.name" :target="item.target" :rel="item.rel" :href="item.href" :class="item.class" class="text-sm/6 font-semibold">{{ item.name }}</a>
          </div>
        </div>
      </nav>
      <dialog class="lg:hidden" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
        <div class="fixed inset-y-0 right-0 z-50 w-2/5 overflow-y-auto bg-gray-800/99 px-6 py-6 sm:max-w-sm">
          <div class="text-end">
            <div class="inline">
              <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = false">
                <span class="sr-only">Close menu</span>
                <svg xmlns="http://www.w3.org/2000/svg" class="text-gray-400 fill-current h-6" alt="Close button" viewBox="0 0 32 32"><g data-name="Layer 2"><path d="M4 29a1 1 0 0 1-.71-.29 1 1 0 0 1 0-1.42l24-24a1 1 0 1 1 1.42 1.42l-24 24A1 1 0 0 1 4 29Z"/><path d="M28 29a1 1 0 0 1-.71-.29l-24-24a1 1 0 0 1 1.42-1.42l24 24a1 1 0 0 1 0 1.42A1 1 0 0 1 28 29Z"/></g><path d="M0 0h32v32H0z" style="fill:none"/></svg></button>
            </div>
          </div>
          <div class="mt-6 flow-root">
            <div class="-my-6 divide-y divide-gray-400/20">
              <div class="py-3">
                <span class="-mx-3 block rounded-lg px-3 py-2.5 text-base/7 font-semibold text-gray-400">Menu</span>
              </div>
              <div class="space-y-2 py-6">
                <a v-for="item in navigation" :key="item.name" :target="item.target" :rel="item.rel" :href="item.href" :class="item.class" class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold hover:bg-gray-900">{{ item.name }}</a>
              </div>
            </div>
          </div>
        </div>
      </dialog>
    </header>
    <div class="mx-auto max-w-2xl">
      <div class="text-center">
        <h1 class="inline text-5xl font-semibold tracking-tight text-balance text-white sm:text-7xl">Welcome to <span class="text-indigo-400">tomhwi01</span>'s site</h1>
        <p class="mt-8 text-lg font-medium text-pretty text-gray-400 sm:text-xl/8">Greetings! My name is Tom.<br />It's a pleasure to share my site with you. I hope you enjoy exploring it!</p>
      </div>
    </div>
  </div>
</template>
  
<script setup lang="ts">
import { ref } from 'vue'

const navigation = [
  { name: 'About me', href: '#about-me', class: 'text-white hover:text-gray-400' },
  { name: 'Projects', href: '#projects', class: 'text-white hover:text-gray-400' },
  { name: 'Contact', href: '#contact', class: 'text-white hover:text-gray-400' },
  { name: 'GitHub', target: '_blank', rel: 'noopener noreferrer', class: 'text-blue-400 hover:text-blue-500', href: 'https://github.com/tomhwi01' },
]

const mobileMenuOpen = ref(false)
</script>