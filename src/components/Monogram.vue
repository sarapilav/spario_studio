<script setup>
import markDark from '../assets/logos/web/mark-dark.png';
import markLight from '../assets/logos/web/mark-light.png';
import panelDark from '../assets/logos/web/logo-panel-dark.png';
import panelLight from '../assets/logos/web/logo-panel-light.png';
import transparentDark from '../assets/logos/web/dark woodmark-transparent.png';

const props = defineProps({
  className: { type: String, default: 'monogram' },
  variant: { type: String, default: 'markLight' },
});

const logos = {
  markDark,
  markLight,
  panelDark,
  panelLight,
  transparentDark,
};
</script>

<template>
  <img :class="className" :src="logos[props.variant] || markLight" alt="" aria-hidden="true">
</template>
