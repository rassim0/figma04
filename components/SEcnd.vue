<template>
  <section class="specialize-section">
    <h2 class="section-title">We Specialize In</h2>

    <NuxtImg
      src="/WHATWE0.png"
      alt="What We Specialize In"
      class="specialize-image"
      format="webp"
    />

    
    <NuxtImg
      src="/WHATWE.png"
      alt="What We Specialize In"
      class="specialize-image01"
      format="webp"
    />

    <p class="section-subtext">And much more...</p>
  </section>
</template>

<script setup>
// No JS needed unless dynamic behavior is added
</script>

<style scoped>
.specialize-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1rem 2rem;
  text-align: center;
  background: #FFFAE5;
  max-width: 1410px;
  margin: 0 auto;
  min-width: 270px;
}

/* Title with clamp for responsiveness */
.section-title {
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: clamp(24px, 5vw, 70px); /* responsive from ~24px to ~40px */
  line-height: 1;
  letter-spacing: 0;
  margin-bottom: 1.5rem;
}

/* Responsive image */
.specialize-image {
  width: 100%;
  max-width: 1000px; /* upper limit to avoid being too big on large screens */
  height: auto;
  margin-bottom: 1.5rem;
}

/* Subtext with clamp and center alignment */
.section-subtext {
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: clamp(15px, 2vw, 35px); /* ~14.4px to ~19.2px */
  line-height: 1;
  letter-spacing: 0;
  text-align: center;


}

.specialize-image01{
    display: none;
}


@media (min-width: 1250px) {
  .specialize-image {
    display: none;
  }

  .specialize-image01 {
    display: block;
    width: 100%;
    max-width: 1100px;
    height: auto;
    margin-bottom: 1.5rem;
  }
}

</style>
