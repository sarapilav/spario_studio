<script setup>
import { ref } from 'vue';
import { navLinks } from '../data.js';
import BrandMark from './BrandMark.vue';

const isOpen = ref(false);
const links = navLinks;

function closeMenu() {
  isOpen.value = false;
}
</script>

<template>
  <header class="site">
    <div class="bar">
      <BrandMark />
      <nav class="primary" :class="{ open: isOpen }" id="primaryNav">
        <a v-for="link in links" :key="link.href" class="nav-link" :href="link.href" @click="closeMenu">{{ link.label }}</a>
        <a href="#contact" class="btn btn-solid" @click="closeMenu">Start a Project</a>
      </nav>
      <button class="nav-toggle" type="button" aria-label="Toggle menu" :aria-expanded="isOpen.toString()" aria-controls="primaryNav" @click="isOpen = !isOpen">☰</button>
    </div>
  </header>
</template>
