<script setup>
import { services } from '../data.js';
import laptopNotes from '../assets/photos/web/laptop-notes.jpg';
import planningTable from '../assets/photos/web/planning-table.jpg';
import workspaceDetail from '../assets/photos/web/workspace-detail.jpg';

const serviceImages = [laptopNotes, planningTable, workspaceDetail, laptopNotes];
</script>

<template>
  <section class="section services-section" id="services">
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

      <div class="services-editorial" aria-label="Services">
        <article
          v-for="(service, index) in services"
          :key="service.number"
          class="service-feature"
          :class="{ 'service-feature-alt': index % 2 === 1 }"
        >
          <div class="service-copy">
            <span class="num">{{ service.number }}</span>
            <h3>{{ service.title }}</h3>
            <p class="row-desc">{{ service.description }}</p>
            <a href="#contact" class="service-link">Discuss this service</a>
          </div>
          <div class="service-media" aria-hidden="true">
            <img :src="serviceImages[index]" alt="">
          </div>
        </article>
      </div>
    </div>
  </section>
</template>
