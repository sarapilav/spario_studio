<script setup>
defineProps({
  eyebrow: { type: String, required: true },
  title: { type: String, required: true },
  description: { type: String, default: '' },
});
</script>

<template>
  <div class="section-head">
    <span class="eyebrow">{{ eyebrow }}</span>
    <h2 class="mt-16" v-html="title"></h2>
    <p v-if="description" class="desc">{{ description }}</p>
  </div>
</template>
