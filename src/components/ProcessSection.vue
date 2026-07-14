<script setup>
import { processStages } from '../data.js';
import SectionHeader from './SectionHeader.vue';
</script>

<template>
  <section class="section" id="process">
    <div class="wrap">
      <SectionHeader eyebrow="The Process" title="From idea to launch, one organized path forward." />
      <div class="stages">
        <div v-for="stage in processStages" :key="stage.tag" class="stage">
          <span class="tag">{{ stage.tag }}</span>
          <h3>{{ stage.title }}</h3>
          <p>{{ stage.text }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
