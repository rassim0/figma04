<template>
  <section class="expandable-section">
    <h2 class="section-title">FAQs</h2>

    <div class="expandable-container">
      <details class="box">
        <summary class="box-header">
          <span class="box-title">How can I use DreamForge to enhance my social media presence?</span>
          <span class="arrow"> <img src="/DAWN.png" /></span>
        </summary>
        <div class="box-description">
          Mindfulify is a mental wellness platform offering guided meditations, articles, and tools to reduce stress and improve focus.
        </div>
      </details>

      <details class="box">
        <summary class="box-header">
          <span class="box-title">How can I use DreamForge to enhance my social media presence?</span>
          <span class="arrow"><img src="/DAWN.png" /></span>
        </summary>
        <div class="box-description">
          Yes, there is a free version available. A premium subscription offers access to more features and content.
        </div>
      </details>

      <details class="box">
        <summary class="box-header">
          <span class="box-title">How can I use DreamForge to enhance my social media presence?</span>
          <span class="arrow"><img src="/DAWN.png" /></span>
        </summary>
        <div class="box-description">
          Simply choose a guided session and find a quiet place. Our sessions are designed for all levels, from beginners to advanced.
        </div>
      </details>

      <details class="box">
        <summary class="box-header">
          <span class="box-title">How can I use DreamForge to enhance my social media presence?</span>
          <span class="arrow"><img src="/DAWN.png" /></span>
        </summary>
        <div class="box-description">
          Currently, Mindfulify requires an internet connection, but offline support is coming soon.
        </div>
      </details>

      <details class="box">
        <summary class="box-header">
          <span class="box-title">How can I use DreamForge to enhance my social media presence?</span>
          <span class="arrow"><img src="/DAWN.png" /></span>
        </summary>
        <div class="box-description">
          You can log in to your dashboard to see your session history, streaks, and personal progress reports.
        </div>
      </details>
    </div>
  </section>
</template>

<style scoped>
.expandable-section {
  max-width: 1355px;
  margin: 0 auto;
  padding: clamp(20px, 5vw, 60px);
  font-family: 'Outfit', sans-serif;
  background: #fffae5;
  min-width: 290px;
  margin-top: -50px;
}

.section-title {
  text-align: center;
  font-size: clamp(24px, 4vw, 42px);
  margin-bottom: clamp(20px, 4vw, 40px);
  font-weight: 600;
}



.box {
  max-width: 1300px;
  border: 1px solid #ccc;
  border-radius: 14px;
  background-color: #ffffff;
  overflow: hidden;
  transition: box-shadow 0.3s ease;
  margin: 0 auto;
  margin-bottom: 10px;
}

.box[open] {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
}

.box summary {

  list-style: none;
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: clamp(12px, 2.5vw, 20px);
  font-size: clamp(12px, 2vw, 28px);
  font-weight: 500;
  color: #ffffff;
  background: #000000;
  transition: background 0.2s ease;
  font-family: 'Poppins';
font-weight: 300;
line-height: 100%;
letter-spacing: 0%;
vertical-align: middle;

}

.box-title {
  max-width: clamp(350px, 60vw, 800px);
}
 
.box summary::-webkit-details-marker {
  display: none;
}

.arrow {
  display: inline-block;
  transition: transform 0.3s ease;
  zoom: 0.7;
}

.arrow :deep(img) {
  width: clamp(16px, 2vw, 28px);
  height: auto;
  display: block;
}

/* Rotate arrow when parent <details> is open */
.box[open] .arrow {
  transform: rotate(180deg);
}

.box-description {
  padding: clamp(10px, 2vw, 18px);
  font-size: clamp(14px, 2vw, 18px);
  line-height: 1.6;
  background: #e0d29b;
  color: #333;
}
</style>
