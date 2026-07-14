<script setup>
import { computed } from 'vue';
import { iconPaths } from '../icons.js';

const props = defineProps({
  name: { type: String, required: true },
  className: { type: String, default: 'icon' },
});

const svgContent = computed(() => iconPaths[props.name] || '');
</script>

<template>
  <svg :class="className" viewBox="0 0 24 24" aria-hidden="true" v-html="svgContent"></svg>
</template>
