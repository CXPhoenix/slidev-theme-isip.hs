<script setup>
import Base from './base.vue'
import SectionImg from '../assets/section_img.svg'
</script>

<template>
  <Base>
    <div class="absolute top-[24%] left-[8%] w-[85%] overflow-hidden page-title z-2" :class="$style.slideSection">
      <slot name="title" />
    </div>
    <div class="absolute top-[36%] left-[9%] w-[84%] overflow-hidden pl-6 z-3" :class="$style.slideSection">
      <slot name="subtitle" />
    </div>
    <img class="absolute top-[46%] left-[47%] w-[55%]" :src="SectionImg" alt="Section Cover">
    <slot />
  </Base>
</template>

<style module lang="postcss">
.slideSection {}

.slideSection :not(h1:first-child):not(h2:first-child) {
  @apply hidden;
}

.slideSection h2 {
  @apply text-4xl pl-6
}
</style>
