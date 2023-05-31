<script setup>
  defineProps({
    id: Number,
    name: String,
    url: String,
  })
</script>

<template>
  <div class="footer">
     <li><a :href="url">{{ name }}</a></li> 
  </div>
  
</template>

<style scoped>
.footer{
  background-color: rgb(215, 164, 146);
  padding-top: -30%;
  padding-left: -30%;
  padding-bottom: -30%;
  padding-right: -30%;
}
</style>
