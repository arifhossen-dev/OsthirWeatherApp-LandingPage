<script setup>
const data = {
  title: 'Boost your productivity. Start using our app today.',
  description: 'Incididunt sint fugiat pariatur cupidatat consectetur sit cillum anim id veniam aliqua proident excepteur commodo do ea.'
}
</script>
<template>
  <div class="bg-white">
    <div class="px-6 py-24 sm:px-6 sm:py-32 lg:px-8">
      <div class="max-w-2xl mx-auto text-center">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl mx-auto max-w-[420px]">
          {{ data.title }}
        </h2>
        <p class="max-w-xl mx-auto mt-6 text-lg leading-8 text-gray-600">
          {{ data.description }}
        </p>
        <div class="flex items-center justify-center mt-10 gap-x-6">
          <a href="#"
            class="rounded-md bg-yellow-400 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-yellow-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
            Get started
          </a>
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Learn more <span
              aria-hidden="true">→</span></a>
        </div>
      </div>
    </div>
  </div>
</template>