<script setup>
import { contactDetails, serviceOptions } from '../data.js';

const details = contactDetails;
</script>

<template>
  <section class="section contact-section" id="contact">
    <div class="wrap contact-wrap">
      <div class="contact-info">
        <span class="eyebrow">Get In Touch</span>
        <h2>Tell us about your business.</h2>
        <p class="desc">Share a few details about your business and what you need, and we'll come back with next steps and a rough plan.</p>
        <div class="contact-detail">
          <div v-for="detail in details" :key="detail.label">
            <span class="label">{{ detail.label }}</span>
            <a v-if="detail.href" :href="detail.href">{{ detail.text }}</a>
            <p v-else>{{ detail.text }}</p>
          </div>
        </div>
      </div>
      <form
        class="contact-form"
        action="https://formsubmit.co/hello@spariostudio.com"
        method="POST"
        aria-label="Contact form"
      >
        <input type="hidden" name="_subject" value="New project enquiry from Spario Studio">
        <input type="hidden" name="_template" value="table">
        <input type="text" name="_honey" class="form-honeypot" tabindex="-1" autocomplete="off" aria-hidden="true">
        <div class="form-row">
          <div>
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
          </div>
          <div>
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
          </div>
        </div>
        <div>
          <label for="service">What do you need?</label>
          <select id="service" name="service" required>
            <option value="" disabled selected>Select a service</option>
            <option v-for="option in serviceOptions" :key="option" :value="option">{{ option }}</option>
          </select>
        </div>
        <div>
          <label for="message">Tell us about your project</label>
          <textarea id="message" name="message" required></textarea>
        </div>
        <button type="submit" class="btn btn-solid">Send Message</button>
      </form>
    </div>
  </section>
</template>
