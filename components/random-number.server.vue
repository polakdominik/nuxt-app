<script setup lang="ts">
const props = defineProps<{ max: number }>();
const rnd = ref(Math.floor(Math.random() * (props.max + 1)));

const alert = () => {
  window.alert('this should not happen');
}
</script>

<template>
  <div class="flex flex-col gap-4">
    <span>{{ rnd }} / {{ props.max }}</span>
    <div><UButton @click="alert">This button should not do anything</UButton></div>
  </div>
</template>
