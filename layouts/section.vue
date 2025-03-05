<script setup>
import Default from './base.vue'
import SectionImg from '../assets/section_img.svg'
</script>

<template>
  <Default>
    <div class="absolute top-[24%] left-[8%] w-[85%] overflow-hidden page-title z-2">
      <slot name="title" />
    </div>
    <div class="absolute top-[35%] left-[9%] w-[84%] overflow-hidden pl-6 z-3">
      <slot name="subtitle" />
    </div>
    <img class="absolute top-[46%] left-[47%] w-[55%]" :src="SectionImg" alt="Section Cover">
    <slot />
  </Default>
</template>
