<script setup>
import { approachItems } from '../data.js';
import AppIcon from './AppIcon.vue';
</script>

<template>
  <section class="section on-navy" id="approach">
    <div class="wrap how-grid">
      <div>
        <span class="eyebrow">How We Work</span>
        <h2 class="mt-16">A clear process, <em class="process-emphasis">from idea to launch.</em></h2>
        <p class="desc mt-22">Every project follows a structured path, so nothing gets lost between planning, building, refining, and launching.</p>
      </div>
      <div class="how-list">
        <div v-for="item in approachItems" :key="item.step" class="how-item">
          <span class="step">{{ item.step }}</span>
          <AppIcon :name="item.icon" />
          <div>
            <h4>{{ item.title }}</h4>
            <p>{{ item.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
