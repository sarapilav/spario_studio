<script setup>
import { navLinks } from '../data.js';
import AppIcon from './AppIcon.vue';
import BrandMark from './BrandMark.vue';

const links = navLinks.filter((link) => link.label !== 'Home');
</script>

<template>
  <footer>
    <div class="wrap footer-top">
      <div>
        <BrandMark variant="dark" />
        <p>A digital studio building websites, software, and the systems behind them, for businesses ready to be taken seriously online.</p>
      </div>
      <div class="footer-col">
        <h5>Studio</h5>
        <a v-for="link in links" :key="link.href" :href="link.href">{{ link.label }}</a>
      </div>
      <div class="footer-col">
        <h5>Get In Touch</h5>
        <a href="mailto:hello@spariostudio.com">hello@spariostudio.com</a>
        <p class="footer-note">Available worldwide - remote first</p>
        <div class="social-links" aria-label="Social links">
          <a href="https://www.instagram.com/" aria-label="Instagram">
            <AppIcon name="instagram" class-name="social-icon" />
          </a>
          <a href="https://www.linkedin.com/" aria-label="LinkedIn">
            <AppIcon name="linkedin" class-name="social-icon" />
          </a>
        </div>
        <a href="#contact" class="btn btn-outline footer-button">Start a Project -></a>
      </div>
    </div>
    <div class="wrap footer-bottom">
      <span>© 2026 Spario Studio. All rights reserved.</span>
      <span>Websites · Software · Content</span>
    </div>
  </footer>
</template>
