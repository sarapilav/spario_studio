<script setup>
import { services } from '../data.js';
</script>

<template>
  <section class="section" id="services">
    <div class="wrap">
      <div class="section-head services-head">
        <div class="head-row">
          <div>
            <span class="eyebrow">What We Do</span>
            <h2 class="mt-16">Services</h2>
          </div>
          <a href="#contact" class="jump">All Services -></a>
        </div>
      </div>

      <div class="services-grid">
        <article v-for="service in services" :key="service.number" class="service-card">
          <span class="num">{{ service.number }}</span>
          <h3>{{ service.title }}</h3>
          <p class="row-desc">{{ service.description }}</p>
        </article>
      </div>
    </div>
  </section>
</template>
