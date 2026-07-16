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
          <h2>Why <em>Spario Studio</em></h2>
          <p class="desc">Spario Studio is a remote-first digital studio based in Sarajevo, Bosnia and Herzegovina, working with clients worldwide.</p>
          <p class="desc">We build websites and custom software from the ground up, shaped around your business instead of forcing your work into a template.</p>
          <ul class="studio-points">
            <li>Custom structure, content, and technical decisions shaped around how your business actually works.</li>
            <li>A defined process with clear milestones, so you always know what is happening next.</li>
            <li>One point of contact from idea to launch, keeping planning, development, and refinement connected.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>
