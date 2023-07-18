<script setup>
const data = {
  imageUrl:'https://cdn.ostad.app//user/avatar/638dc11391cbb43930e05dd1',
  linkUrl:'https://ostad.app/instructor/16838'
}
</script>

<template>

  <div>
    <a :href="data.linkUrl">
      <img :src="data.imageUrl" alt="Hasin Hayder on Ostad">
    </a>
  </div>
  
</template>