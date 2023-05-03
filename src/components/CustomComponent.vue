<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
 <div class="custom-component">
  <div class="title text-center">
    i'm a custom component!
  </div>
 </div>
</template>

<style scoped>
  .title {
    font-size: 1em;
  }
</style>
