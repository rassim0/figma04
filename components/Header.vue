<template>
  <div class="header-wrapper">
    <!-- Navbar Section -->
    <div class="navbar">
      <NuxtImg src="/LOGO.png" alt="Logo" class="logo" />

      <button class="menu-button" @click="toggleSidebar">
  Menu
</button>
<!-- Desktop navigation links (visible ≥842px only via CSS) -->
<div class="desktop-nav-links">
  <NuxtLink to="/" class="nav-link">Home</NuxtLink>
  <NuxtLink to="/about" class="nav-link">About Us</NuxtLink>
  <NuxtLink to="/products" class="nav-link">Products</NuxtLink>
  <NuxtLink to="/pricing" class="nav-link">Pricing</NuxtLink>
</div>

<!-- Desktop download button -->
<button class="download-button">
  Download <NuxtImg src="/download.png" class="down" />
</button>
    </div>

    <!-- Sidebar -->
    <transition name="slide">
      <div v-if="sidebarOpen" class="sidebar">
        <button class="close-button" @click="toggleSidebar">×</button>
        <nav class="sidebar-nav">
          <NuxtLink to="/" class="nav-link">Home</NuxtLink>
          <NuxtLink to="/about" class="nav-link">About Us</NuxtLink>
          <NuxtLink to="/products" class="nav-link">Products</NuxtLink>
          <NuxtLink to="/pricing" class="nav-link">Pricing</NuxtLink>
        </nav>
      </div>
    </transition>

    <!-- Title + Description -->
    <div class="hero-content">
      <h1 class="hero-title">Embrace mindfulness,<br>
one click at a time.</h1>
      <p class="hero-description">
        Your digital landscape where <br> mindfulness and well-being meet.
      </p>
    </div>

    <!-- Images Row -->
    <div class="hero-image-wrapper">
    <NuxtImg src="/BIG1.png" alt="Main Image" class="hero-image big" />

    <NuxtImg src="/Small11.png" alt="Top Right" class="hero-image small top-right" />

    <NuxtImg src="/Small22.png" alt="Bottom Left" class="hero-image small bottom-left" />
  </div>
 



  <!-- Video Section -->
<div class="video-wrapper">
  <!-- Placeholder image with icons -->
  <div class="video-placeholder">
    <img src="/CER.png" alt="Video Placeholder" class="video-poster" />
    <img src="/PL.png" alt="Play Icon" class="play-icon" />
  </div>

  <!-- Actual video (optional autoplay or controls) -->
  <video class="video-player" controls poster="/DATA.png">
    <source src="/supercar.mp4" type="video/mp4" />

  </video>
 </div>

</div>
 
</template>

<script setup>
import { ref } from 'vue'

const sidebarOpen = ref(false)
const toggleSidebar = () => {
  sidebarOpen.value = !sidebarOpen.value
}
</script>

<style scoped>




.video-wrapper {
  width: 100%;
  max-width: 1250px;
  margin-inline: auto;
  position: relative;
   aspect-ratio: 16 / 9;
   margin-top: -10px;
}

.video-placeholder {
  position: absolute;
  width: 100%;
  aspect-ratio: 16 / 9;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 2;
  top: clamp(20px, 1.5vw, 40px);
}

.video-poster {
  width: 18%;
  height: auto;
  object-fit: cover;
}

.play-icon {
  position: absolute;
  width: 5%;
  height: auto;
  z-index: 2;
}

.video-player {
  background: #000000;
  width: 100%;
  min-height: 240px;
  height: 100%;
  border-radius: 15px;
}



/* Basic Layout */
.header-wrapper {
  max-width: 1000px;
  min-width: 300px;
  display: flex;
  flex-direction: column;
  padding: 16px;
  background: #FFFAE5;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 10px;
}

.logo {
  width: 100px;
  height: auto;
  zoom: 1.2;
}

.menu-button {
  background: #FAC97A;
  color: #000000;
  border: none;
  font-size: 14px;
  padding: 5px 18px;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.2s ease;
font-weight: 400;
line-height: 100%;
letter-spacing: 0%;
text-align: center;
font-family: 'Clash Display Variable', sans-serif;
}
 

/* Sidebar */
.sidebar {
  position: fixed;
  top: 0;
  right: 0;
  width: 75%;
  height: 100%;
  background-color: rgb(216, 212, 156);
  box-shadow: -19px 6px 7px rgba(19, 17, 17, 0.1);
  z-index: 1000;
  padding: 25px;
  display: flex;
  flex-direction: column;
}

.sidebar-nav {
  display: flex;
  flex-direction: column;
  gap: 26px;
  margin-top: 32px;
}

.nav-link {
  text-decoration: none;
  color: #000000;
  font-weight: bold;
  font-family: 'Outfit', sans-serif;
}

.close-button {
  align-self: flex-end;
  font-size: 38px;
  background: none;
  border: none;
  cursor: pointer;
}

/* Transition */
.slide-enter-active,
.slide-leave-active {
  transition: transform 0.3s ease;
}
.slide-enter-from {
  transform: translateX(100%);
}
.slide-leave-to {
  transform: translateX(100%);
}



.hero-content {
  margin-top: 32px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

/* Title */
.hero-title {
  font-size: clamp(24px, 8vw, 120px);  /* scales with screen size */
  margin-bottom: -5px;
  max-width: 100%;
  font-family: 'Outfit';
font-weight: 900;
line-height: 100%;
letter-spacing: 0%;
text-align: center;
}

/* Description */
.hero-description {
  font-size: clamp(14px, 5vw, 90px); /* responsive */
  color: #000000;
  width: 100%;
font-weight: 200;
line-height: 100%;
letter-spacing: 0%;
text-align: center;
font-family: 'Clash Display', sans-serif;
}



/* Image Row */
.hero-image-wrapper {
  position: relative;
  width: 100%;
  max-width: 1000px;
  margin: 0 auto;
  aspect-ratio: 1 / 1; /* Makes the wrapper square */

}

.hero-image {
  max-width: 100%;
  height: auto;
  display: block;
}

.hero-image.big {
  min-width: 141px;
  max-width:733px ;
  width: 80%;
  height: auto;
  object-fit: cover;
  position: relative;
  top: 40px;
  left: 30px;
}

.hero-image.small {
  position: absolute;
  width: 30%;  
  height: auto;
  object-fit: contain;
}

.top-right {
  margin-right: 30px;
  top: 80px;
  right: 30px;
  transform: translate(25%, -25%);
}

.bottom-left {
  left: 25px;
  transform: translate(-25%, 25%);
  margin-left: 20px;
}

/* Center container + max-width */
.header-wrapper {
  max-width: 1440px;
  margin: 0 auto;
}

/* Desktop nav links and download button - hidden by default */
.desktop-nav-links,
.download-button {
  display: none;
}

/* Media query for screens ≥842px */
@media (min-width: 842px) {
  
/* Description */
.hero-description {
  font-size: clamp(14px, 3.5vw, 60px); /* responsive */
  
}


.video-player {
    border-radius: 50px;
  }

}



@media (min-width: 1250px) {
  .hero-image-wrapper {
  left: 100px;
}

.header-wrapper{
  max-width: 1440px;
}

  .top-right {
    margin-right: 20px;
  top: 120px;
  right: 130px;
  transform: scale(1.2) translate(25%, -25%);
}

.bottom-left {
  top: 509px;
  left: -95px;
  transform: scale(1.2) translate(25%, -25%);
}


.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
    margin-left: 30px;
    margin-right: 30px;
  }

  .menu-button {
    display: none; /* hide menu button on desktop */
  }

  .desktop-nav-links {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 32px;
    flex-grow: 1;
  }

  .desktop-nav-links .nav-link {
    font-weight: 200;
    text-decoration: none;
    color: #000000;
    font-size: 35px;
line-height: 100%;
letter-spacing: 0%;
 font-family: 'Clash Display', sans-serif;
  }

  .download-button {
    display: inline-block;
    background: #FAC97A;
    color: #000000;
    border: none;
    font-size: 26px;
    padding: 8px 16px;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color 0.2s ease;
  }

  .down {
    zoom: 1.2;
    margin-left: 3px;
  }
  .logo {
  width: 100px;
  height: auto;
  zoom: 2;
}

 .top-right {
    margin-right: 20px;
  top: 120px;
  right: 70px;
}

.bottom-left {
  top: 509px;
  left: -95px;
  transform: translate(-25%, 25%);
}


.video-wrapper {
   margin-top: -100px;
}
}

 
</style>
