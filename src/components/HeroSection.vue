<script setup>
import heroWorkspace from '../assets/photos/web/laptop-notes.jpg';
import Monogram from './Monogram.vue';
</script>

<template>
  <section class="hero" id="top">
    <div class="hero-inner">
      <div>
        <span class="eyebrow">A Digital Studio · Est. 2026</span>
        <h1>Custom digital solutions,<br><em>from idea to launch.</em></h1>
        <p class="lede">Spario Studio helps businesses build websites, custom software, integrations, and content through a clear, complete, and practical process.</p>
        <p class="lede lede-secondary">From planning and structure to development, refinement, and launch - we create digital solutions designed around your business needs.</p>
        <div class="cta-row">
          <a href="#contact" class="btn btn-solid">Start a Project</a>
          <a href="#contact" class="btn btn-outline">Contact Us</a>
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
