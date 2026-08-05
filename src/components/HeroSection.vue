<script setup>
import heroWorkspace from '../assets/photos/web/laptop-notes.jpg';
import Monogram from './Monogram.vue';
</script>

<template>
  <section class="hero" id="top">
    <div class="hero-inner">
      <div>
        <span class="eyebrow">Digital Studio · Sarajevo → Worldwide</span>
        <h1>Custom digital solutions,<br><em>built around your business.</em></h1>
        <p class="lede">We design and build websites, webshops, software, and the content that supports them — for small and medium businesses and first-time founders ready to be taken seriously online.</p>
        <div class="cta-row">
          <a href="#contact" class="btn btn-solid">Start a Project</a>
          <a href="#services" class="btn btn-outline">Explore Services</a>
        </div>
      </div>
      <div class="hero-visual" role="img" aria-label="Workspace with a laptop, notes, and coffee">
        <img class="hero-visual-image" :src="heroWorkspace" alt="">
        <div class="frame">
          <Monogram class-name="hero-logo-overlay" variant="transparentDark" />
        </div>
      </div>
    </div>
  </section>
</template>
