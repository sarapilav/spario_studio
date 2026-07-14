<script setup>
import { tickerItems } from '../data.js';

const items = tickerItems;
</script>

<template>
  <div class="ticker">
    <div class="ticker-inner">
      <span v-for="item in items" :key="item">{{ item }}</span>
    </div>
  </div>
</template>
