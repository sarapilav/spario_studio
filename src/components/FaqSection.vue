<script setup>
import { faqs } from '../data.js';
import SectionHeader from './SectionHeader.vue';
</script>

<template>
  <section class="section" id="faq">
    <div class="wrap">
      <SectionHeader eyebrow="Good to Know" title="Questions worth answering upfront." />
      <div class="faq-list">
        <details v-for="faq in faqs" :key="faq.question" :open="faq.open">
          <summary>{{ faq.question }} <span class="plus">+</span></summary>
          <p>{{ faq.answer }}</p>
        </details>
      </div>
    </div>
  </section>
</template>
