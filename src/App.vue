<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import { Carousel } from "ant-design-vue";
</script>

<template>
  <Carousel>
    <HelloWorld msg="Test A" />
    <HelloWorld msg="Test B" />
  </Carousel>
</template>
