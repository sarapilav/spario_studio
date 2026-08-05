<script setup>
import { reasonsToChooseUs } from '../data.js';
import SectionHeader from './SectionHeader.vue';
</script>

<template>
  <section class="section testimonials-section" id="why-us">
    <div class="wrap">
      <div class="testimonials-head">
        <SectionHeader
          eyebrow="Why Spario Studio"
          title="A focused partner, from first idea to launch."
          description="Clear communication, thoughtful decisions, and solutions shaped around the way your business actually works."
        />
        <a href="#contact" class="btn btn-outline">Request Examples</a>
      </div>

      <div class="testimonial-grid">
        <article v-for="(reason, index) in reasonsToChooseUs" :key="reason.title" class="testimonial-card">
          <span class="eyebrow">0{{ index + 1 }}</span>
          <h3>{{ reason.title }}</h3>
          <p class="quote">{{ reason.text }}</p>
        </article>
      </div>
    </div>
  </section>
</template>
