<template>
  <section class="horizontal-card-wrapper">
    <h2 class="horizontal-card-title">Stay informed about mental health<br> with the latest insights from our blog</h2>

    <div class="horizontal-card-section">
      <div class="horizontal-card">
        <p class="card-date">December 2023</p>
        <h3 class="card-title">10 Daily Habits for Cultivating Mindfulness</h3>
        <img class="card-image" src="/PHOTO01.png" alt="DreamForge Preview" />
      </div>

      <div class="horizontal-card">
        <p class="card-date">January 2024</p>
        <h3 class="card-title">The Pure Science of <br> Happiness</h3>
        <img class="card-image" src="/PHOTO02.png" alt="AI Future" />
      </div>
    </div>
  </section>
</template>

<style scoped>

.horizontal-card-wrapper {
  background: #fffae5;
  padding: clamp(30px, 5vw, 60px) 0;
  max-width: 1475px;
  margin: 0 auto;
  box-sizing: border-box;
  margin-top: -30px;
  min-width: 330px;
}

.horizontal-card-title {
  text-align: center;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: clamp(20px, 4.5vw, 65px);
  color: #000000;
  margin-bottom: clamp(24px, 4vw, 60px);
}


.horizontal-card-section {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: clamp(16px, 4vw, 48px);
  padding: clamp(20px, 5vw, 60px);
  max-width: 1475px;
  min-width: 330px;
  margin: 0 auto;
  box-sizing: border-box;
  background: #fffae5;
  flex-wrap: nowrap; /* Forces cards to stay side by side */
  overflow-x: auto;   /* Allow scroll if screen is too small */
  margin-top: -20px;
}

.horizontal-card {
  flex: 0 0 clamp(140px, 46.5%, 800px); /* Always occupy less than 50% */
  background: #000000;
  border-radius: 20px;
  padding: clamp(16px, 3vw, 32px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  box-sizing: border-box;
}

.card-date {
  font-size: clamp(10px, 1.5vw, 25px);
  color: #B1B1B1;
  margin-bottom: clamp(8px, 1vw, 12px);
  font-family: 'Outfit';
  font-weight: 300;
  line-height: 100%;
  letter-spacing: 0%;
  text-align: center;
  vertical-align: middle;
}

.card-title {
  font-size: clamp(10px, 2.7vw, 50px);
  font-weight: 600;
  margin-bottom: clamp(12px, 2vw, 20px);
  color: #B1B1B1;
  font-family: 'Outfit';
  font-weight: 500;
  line-height: 100%;
  letter-spacing: 0%;
  text-align: center;
  vertical-align: middle;
  margin-top: 20px;
}


.card-image {
  width: 100%;
  height: auto;
  border-radius: 8px;
  object-fit: cover;
  margin-top: 10px;
}
</style>
