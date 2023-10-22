<script setup>
import { buttonVariants } from ".";
import { cn } from "src/lib/utils";

withDefaults(defineProps(), {
  as: "button",
});
</script>

<template>
  <component
    :is="as"
    :class="cn(buttonVariants({ variant, size }), $attrs.class ?? '')"
  >
    <slot />
  </component>
</template>
