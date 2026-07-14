<script setup>
import { testimonials } from '../data.js';
import SectionHeader from './SectionHeader.vue';
</script>

<template>
  <section class="section testimonials-section" id="testimonials">
    <div class="wrap">
      <div class="testimonials-head">
        <SectionHeader
          eyebrow="Client Notes"
          title="Quiet proof, shared with care."
          description="If you want to see relevant project examples, get in touch and we will send selected work privately."
        />
        <a href="#contact" class="btn btn-outline">Request Examples</a>
      </div>

      <div class="testimonial-grid">
        <article v-for="testimonial in testimonials" :key="testimonial.quote" class="testimonial-card">
          <p class="quote">“{{ testimonial.quote }}”</p>
          <div class="testimonial-source">
            <span>{{ testimonial.name }}</span>
            <small>{{ testimonial.company }}</small>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>
