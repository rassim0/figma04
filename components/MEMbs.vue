<template>
  <section class="slider-section">
    <!-- Title -->
    <h2 class="slider-title">Our Network of <span class="hkk">700+</span> <br> licensed therapists</h2>

    <!-- Swiper Slider -->
    <Swiper
      :modules="[Navigation]"
      :slides-per-view="2"
      :space-between="20"
      :allow-touch-move="true"
      
      @slideChange="onSlideChange"
      class="testimonial-swiper"
    >
      <!-- Slide 1 -->
      <SwiperSlide>
        <div class="slide-content">
          <NuxtImg src="/PIC1.png" alt="Joe Bush" class="testimonial-image" loading="lazy" />
          <p class="testimonial-name">Dr. Maya Patel, 38</p>
          <p class="testimonial-role">Psychiatrist</p>
          <div class="testimonial-special">
            <p class="special-title">Specializes in - <br>Mood disorders, anxiety disorders</p>
            <p class="testimonial-description">
              “Compassionate, holistic approach, evidence-based treatments”
            </p>
          </div>
        </div>
      </SwiperSlide>

      <!-- Slide 2 -->
      <SwiperSlide>
        <div class="slide-content">
          <NuxtImg src="/PIC2.png" alt="Anna Kim" class="testimonial-image" loading="lazy" />
          <p class="testimonial-name">Dr. Deep Naik, 35</p>
          <p class="testimonial-role">Clinical Psychiatrist</p>
          <div class="testimonial-special">
            <p class="special-title">Specializes in - <br>
CBT, Trauma therapy</p>
            <p class="testimonial-description">
              “Empathetic, solution-focused, trauma-informed care”
            </p>
          </div>
        </div>
      </SwiperSlide>

      <!-- Slide 3 -->
      <SwiperSlide>
        <div class="slide-content">
          <NuxtImg src="/PIC3.png" alt="Michael Ray" class="testimonial-image" loading="lazy" />
          <p class="testimonial-name">Dr. Kayla Andrews, 30</p>
          <p class="testimonial-role">Psychiatrist</p>
          <div class="testimonial-special">
            <p class="special-title">Specializes in - <br>
Pediatric mental health</p>
            <p class="testimonial-description">
              “Patient-centred, integrative and mindfulness-based interventions”
            </p>
          </div>
        </div>
      </SwiperSlide>

      <!-- Slide 4 -->
      <SwiperSlide>
        <div class="slide-content">
          <NuxtImg src="/PIC1.png" alt="Joe Bush" class="testimonial-image" loading="lazy" />
          <p class="testimonial-name">Dr. Maya Patel, 38</p>
          <p class="testimonial-role">Psychiatrist</p>
          <div class="testimonial-special">
            <p class="special-title">Specializes in -<br> 
Mood disorders, anxiety disorders</p>
            <p class="testimonial-description">
              “Compassionate, holistic approach, evidence-based treatments”
            </p>
          </div>
        </div>
      </SwiperSlide>

      <!-- Slide 5 -->
      <SwiperSlide>
        <div class="slide-content">
          <NuxtImg src="/PIC3.png" alt="Michael Ray" class="testimonial-image" loading="lazy" />
          <p class="testimonial-name">Dr. Kayla Andrews, 30</p>
          <p class="testimonial-role">Psychiatrist</p>
          <div class="testimonial-special">
            <p class="special-title">Specializes in - <br>
Pediatric mental health</p>
            <p class="testimonial-description">
              “Patient-centred, integrative and mindfulness-based interventions”
            </p>
          </div>
        </div>
      </SwiperSlide>
    </Swiper>


    <!-- Swiper Slider for desktop (only visible on screens ≥1200px) -->
<Swiper
  :modules="[Navigation]"
  :slides-per-view="3"
  :space-between="20"
  :allow-touch-move="true"
  @slideChange="onSlideChange"
  class="testimonial-swiper desktop-swiper"
>
  <!-- Slide 1 -->
  <SwiperSlide>
    <div class="slide-content">
      <NuxtImg src="/PIC1.png" alt="Joe Bush" class="testimonial-image" loading="lazy" />
      <p class="testimonial-name">Dr. Maya Patel, 38</p>
      <p class="testimonial-role">Psychiatrist</p>
      <div class="testimonial-special">
        <p class="special-title">Specializes in - <br>Mood disorders, anxiety disorders</p>
        <p class="testimonial-description">
          “Compassionate, holistic approach, evidence-based treatments”
        </p>
      </div>
    </div>
  </SwiperSlide>

  <!-- Slide 2 -->
  <SwiperSlide>
    <div class="slide-content">
      <NuxtImg src="/PIC2.png" alt="Anna Kim" class="testimonial-image" loading="lazy" />
      <p class="testimonial-name">Dr. Deep Naik, 35</p>
      <p class="testimonial-role">Clinical Psychiatrist</p>
      <div class="testimonial-special">
        <p class="special-title">Specializes in - <br>CBT, Trauma therapy</p>
        <p class="testimonial-description">
          “Empathetic, solution-focused, trauma-informed care”
        </p>
      </div>
    </div>
  </SwiperSlide>

  <!-- Slide 3 -->
  <SwiperSlide>
    <div class="slide-content">
      <NuxtImg src="/PIC3.png" alt="Michael Ray" class="testimonial-image" loading="lazy" />
      <p class="testimonial-name">Dr. Kayla Andrews, 30</p>
      <p class="testimonial-role">Psychiatrist</p>
      <div class="testimonial-special">
        <p class="special-title">Specializes in - <br>Pediatric mental health</p>
        <p class="testimonial-description">
          “Patient-centred, integrative and mindfulness-based interventions”
        </p>
      </div>
    </div>
  </SwiperSlide>

  <!-- Slide 4 -->
  <SwiperSlide>
    <div class="slide-content">
      <NuxtImg src="/PIC1.png" alt="Joe Bush" class="testimonial-image" loading="lazy" />
      <p class="testimonial-name">Dr. Maya Patel, 38</p>
      <p class="testimonial-role">Psychiatrist</p>
      <div class="testimonial-special">
        <p class="special-title">Specializes in - <br>Mood disorders, anxiety disorders</p>
        <p class="testimonial-description">
          “Compassionate, holistic approach, evidence-based treatments”
        </p>
      </div>
    </div>
  </SwiperSlide>

  <!-- Slide 5 -->
  <SwiperSlide>
    <div class="slide-content">
      <NuxtImg src="/PIC3.png" alt="Michael Ray" class="testimonial-image" loading="lazy" />
      <p class="testimonial-name">Dr. Kayla Andrews, 30</p>
      <p class="testimonial-role">Psychiatrist</p>
      <div class="testimonial-special">
        <p class="special-title">Specializes in - <br>Pediatric mental health</p>
        <p class="testimonial-description">
          “Patient-centred, integrative and mindfulness-based interventions”
        </p>
      </div>
    </div>
  </SwiperSlide>
</Swiper>

    <!-- Slide Counter -->
    <div class="slide-counter">
      {{ currentSlide + 1 }}/05
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Navigation } from 'swiper/modules'
import 'swiper/css'
import 'swiper/css/navigation'

const currentSlide = ref(0)

const onSlideChange = (swiper) => {
  currentSlide.value = swiper.realIndex
}
</script>

<style scoped>

.slider-section {
 min-width: 300px;
  padding: 2rem 1rem;
  position: relative;
  background: #FFFAE5;
  max-width: 1440px;
  margin: 0 auto;
  margin-bottom: 30px;
 padding-bottom: 40px;
 margin-top: -30px;
}

.slider-title {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(24px, 4vw, 48px);
  font-weight: 600;
  text-align: center;
  margin-bottom: 2rem;
line-height: 100%;
letter-spacing: 0%;
vertical-align: middle;

}

.hkk{
    font-weight: 900;
}

.testimonial-swiper {
  width: 100%;
}

.swiper-slide {
  display: flex;
  height: auto !important;
}


.testimonial-swiper .swiper-wrapper {
  display: flex;
  justify-content: center !important;
}


.slide-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #000000;
  border-radius: 12px;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  margin-bottom: 10px;
  border-radius: 22px;
  max-width:342px; 
  align-items: flex-start;
  text-align: left;
}


.testimonial-image {
  align-self: center;
  width: 100%;
  max-width: 315px;
  object-fit: cover;
  border-radius: 8px;
  margin-top: clamp(0.1rem, 1vw, 1rem);
}

.testimonial-name {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(12px, 2vw, 20px);
  font-weight: 600;
  margin-bottom: -0.25rem;
  line-height: 100%;
  letter-spacing: 0%;
  vertical-align: middle;
  color: #FFFFFF;
  text-align: left;
}

.testimonial-role {
  font-size: clamp(10px, 2.5vw, 20px);
  color: #ffffff;
  margin-bottom: 1rem;
  font-family: 'Outfit', sans-serif;
  font-weight: 400;
  line-height: 100%;
  letter-spacing: 0%;
  vertical-align: middle;
  text-align: left;
 margin-bottom: 0rem;
}

.special-title {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(10px, 2vw, 18px);
  color: #acabab;
  font-weight: 100;
  line-height: 140%;
  letter-spacing: 0%;
  vertical-align: middle;
  text-align: left;
}

.testimonial-description {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(10px, 2vw, 18px);
  color: #acabab;
  font-weight: 100;
  line-height: 100%;
  letter-spacing: 0%;
  vertical-align: middle;
  text-align: left;
   margin-bottom: 0.2rem;
}

.testimonial-name,
.testimonial-role,
.special-title,
.testimonial-description {
  margin-left: clamp(0.5rem, 1vw, 1rem);
}

.slide-counter {
  position: absolute;
  bottom: 1rem;
  left: 1rem;
  font-family: 'Outfit', sans-serif;
  font-size: clamp(14px, 1vw, 18px);
font-weight: 600;
line-height: 100%;
letter-spacing: 0%;
vertical-align: middle;
}

.desktop-swiper {
  display: none;
}

@media(min-width: 850px){
.testimonial-swiper {
margin-left: clamp(0.5rem, 4.5vw, 10rem);
}

.testimonial-swiper {
  width: 90%;
}


}

@media (min-width: 1200px) {
  .testimonial-swiper {
    display: none;

  }
  .desktop-swiper {
    display: block;
  }


  .slide-counter {
  position: absolute;
  left:clamp(0.5rem, 5.5vw, 12rem);
}

}
</style>
