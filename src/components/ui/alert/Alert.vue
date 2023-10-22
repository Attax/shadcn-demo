<script setup>
import { alertVariants } from ".";
import { cn } from "@/lib/utils";

const props = defineProps();
</script>

<template>
  <div :class="cn(alertVariants({ variant }), props.class ?? '')">
    <slot />
  </div>
</template>
