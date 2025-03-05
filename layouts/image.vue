<script setup>
import Base from './base.vue'
</script>

<template>
  <Base>
    <div class="absolute top-[9%] left-[7%] w-[86%] h-[12%]">
      <div class="flex justify-center item-center h-full page-title overflow-hidden">
        <slot name="title" />
      </div>
    </div>
    <div class="absolute top-[21%] left-[7%] w-[86%] h-[65%] overflow-hidden">
      <div :class="$style.image">
        <slot />
      </div>
    </div>
  </Base>
</template>

<style module lang="postcss">
.image {
  @apply w-full h-full p-4;
}

.image > p {
  @apply flex justify-center items-center h-full
}
</style>