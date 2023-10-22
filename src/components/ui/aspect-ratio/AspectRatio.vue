<script setup>
import { AspectRatio } from "radix-vue";

const props = defineProps();
</script>

<template>
  <AspectRatio v-bind="props">
    <slot />
  </AspectRatio>
</template>
