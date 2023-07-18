<script setup>
import { ref } from "vue"

let isOnTop = ref(false)


window.onscroll = function () {
  if (document.body.scrollTop > 200 || document.documentElement.scrollTop > 200) {
    isOnTop.value = true
  } else {
    isOnTop.value = false
  }
}


const scrollToTop = () => {
  window.scrollTo({ top: 0, left: 0, behavior: 'smooth' });
}
</script>
<template>
  <button @click="scrollToTop" :class="isOnTop ? 'flex' : 'hidden'"
    class="fixed items-center justify-center w-8 h-16 text-3xl font-bold text-green-600 bg-yellow-300 rounded-full ring-4 ring-offset-4 ring-yellow-400 z-90 bottom-8 right-8">

    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
      class="w-10 h-10">
      <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 6.75L12 3m0 0l3.75 3.75M12 3v18" />
    </svg>

  </button>
</template>