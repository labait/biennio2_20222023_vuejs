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
  <div class="title">
    i'm a custom component!
  </div>
 </div>
</template>

<style scoped>
  .title {
    font-size: 2em;
  }
</style>
