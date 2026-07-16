<script setup>
const stats = [
  { value: '01', label: 'Point of contact from idea to launch' },
  { value: '05', label: 'Clear project stages from planning to release' },
  { value: '24h', label: 'Typical response within one business day' },
];
</script>

<template>
  <section class="stats-band" aria-label="Project highlights">
    <div class="wrap stats-grid">
      <div v-for="stat in stats" :key="stat.value" class="stat-item">
        <strong>{{ stat.value }}</strong>
        <span>{{ stat.label }}</span>
      </div>
    </div>
  </section>
</template>
