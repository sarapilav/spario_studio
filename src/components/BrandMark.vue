<script setup>
import logoDark from '../assets/logos/web/logo-horizontal-dark.png';
import logoLight from '../assets/logos/web/logo-horizontal-light.png';

const props = defineProps({
  variant: { type: String, default: 'light' },
});

const logos = {
  light: logoLight,
  dark: logoDark,
};
</script>

<template>
  <a href="#top" class="mark" aria-label="Spario Studio home">
    <img class="mark-logo" :src="logos[props.variant] || logoLight" alt="" aria-hidden="true">
  </a>
</template>
