<script setup>
import planningTable from '../assets/photos/web/planning-table.jpg';
import workspaceDetail from '../assets/photos/web/workspace-detail.jpg';
</script>

<template>
  <section class="section studio" id="studio">
    <div class="wrap">
      <div class="studio-grid">
        <div class="studio-aside">
          <span class="eyebrow">The Studio</span>
          <div class="studio-collage" aria-hidden="true">
            <img class="studio-collage-main" :src="planningTable" alt="">
            <img class="studio-collage-small" :src="workspaceDetail" alt="">
            <div class="studio-collage-note">
              <span>Remote first</span>
              <strong>Sarajevo / Worldwide</strong>
            </div>
          </div>
        </div>
        <div>
          <h2>Small studio, <em>full attention.</em></h2>
          <p class="desc">Spario Studio is a remote-first digital studio based in Sarajevo, Bosnia and Herzegovina, working with clients worldwide.</p>
          <p class="desc">We build websites and custom software from the ground up, shaped around your business instead of forcing your work into a template.</p>
          <ul class="studio-points">
            <li>You get a plan that fits your business — not a template stretched to cover it.</li>
            <li>Clear milestones at every stage, so you always know what is happening next.</li>
            <li>One person to talk to, from first call to launch day.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>
