<script setup lang="ts">
import { onBeforeUnmount, onMounted, onUnmounted } from "vue";

const props = defineProps<{ msg: string }>();

onMounted(() => {
  console.log(`onMounted: ${props.msg}`);
});

onBeforeUnmount(() => {
  console.log(`onBeforeUnmount: ${props.msg}`);
});

onUnmounted(() => {
  console.log(`onUnmounted: ${props.msg}`);
});
</script>

<template>
  <h1>{{ msg }}</h1>
</template>
