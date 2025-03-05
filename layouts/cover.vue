<script setup>
import Section from './section.vue';
import IsipImg from '../assets/isip_slogon.svg'
</script>

<template>
  <Section>
    <div class="absolute top-[24%] left-[8%] w-[85%] overflow-hidden page-title z-2 text-center">
      <slot name="title" />
    </div>
    <div class="absolute top-[35%] left-[8%] w-[85%] overflow-hidden z-3 text-center">
      <slot name="subtitle" />
    </div>
    <img :src="IsipImg" alt="isip-hs title" class="absolute top-[56%] left-[1%] w-[42%]">
  </Section>
</template>
