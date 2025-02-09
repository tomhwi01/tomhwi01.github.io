<template>
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
    <div class="mx-auto max-w-2xl py-16 sm:py-24 lg:max-w-none lg:py-32">
      <a name="projects"><h2 class="text-2xl font-bold text-white">Projects</h2></a>
      <div class="mt-6 space-y-12 lg:grid lg:grid-cols-3 lg:gap-x-6 lg:space-y-0">
        <div v-for="callout in callouts" :key="callout.name" class="group">
          <a :href="callout.href" target="_blank" rel="noopener noreferrer">
            <img :src="callout.imageSrc" :alt="callout.imageAlt" type="image/jpeg" class="w-full rounded-lg bg-white object-cover group-hover:opacity-75 max-sm:h-80 sm:aspect-2/1 lg:aspect-square" />
            <h3 class="mt-6 text-base font-semibold text-white">
                {{ callout.name }}
            </h3>
          </a>
            <p class="text-sm text-gray-400">{{ callout.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import siteImg from '../assets/site.jpeg'
import webPageImg from '../assets/webpage.jpeg'
import testResultImg from '../assets/test_result.jpeg'
import sudokuImg from '../assets/sudoku.jpeg'
const callouts = [
  {
    name: 'My Site',
    description: 'Built with Vue 3 + TypeScript + Vite + Tailwind CSS',
    imageSrc: siteImg,
    imageAlt: 'My Site GitHub page',
    href: 'https://github.com/tomhwi01/tomhwi01.github.io',
  },
  {
    name: 'Dog Human Classifier',
    description: 'Built with Python + TensorFlow + Keras + Flask + HTML5',
    imageSrc: webPageImg,
    imageAlt: 'Dog Human Classifier GitHub page',
    href: 'https://github.com/tomhwi01/dog-human-classifier',
  },
  {
    name: 'Audio Classifier',
    description: 'Built with Python + TensorFlow + Keras',
    imageSrc: testResultImg,
    imageAlt: 'Audio Classifier GitHub page',
    href: 'https://github.com/tomhwi01/audio_classification',
  },
  {
    name: 'Sudoku Solver',
    description: 'Built with Java',
    imageSrc: sudokuImg,
    imageAlt: 'Sudoku Solver GitHub page',
    href: 'https://github.com/tomhwi01/sudoku',
  },
]
</script>