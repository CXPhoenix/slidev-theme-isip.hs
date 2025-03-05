<script setup>
import Default from './base.vue'
</script>

<template>
  <Default>
    <div class="absolute top-[9%] left-[7%] w-[86%] h-[12%]">
      <div class="flex justify-center item-center h-full page-title overflow-hidden">
        <slot name="title" />
      </div>
    </div>
    <div class="absolute top-[21%] left-[7%] w-[86%] h-[65%] overflow-hidden">
      <slot />
    </div>
  </Default>
</template>
