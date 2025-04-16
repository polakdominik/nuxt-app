<script setup lang="ts">
const count = ref(100);
</script>

<template>
  <div class="flex flex-col gap-4">
    <div><UButton @click="count++">Increment</UButton></div>
    <RandomNumber :max="count"/>
  </div>
</template>
