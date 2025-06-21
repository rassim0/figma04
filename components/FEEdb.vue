<template>
  <div class="cards-section">
    <!-- Title Block -->
    <div class="cards-header">
      <h2 class="cards-title">Words speaks for us</h2>
    </div>

    <!-- Cards Block -->
    <div class="cards-container">
      <div class="card card-1">              <br>     <br>    <br>    <br>    <br>    <br>    <br>                    </div>
      <div class="card card-2">               <br>    <br>    <br>    <br>    <br>    <br>    <br>   </div>
      <div class="card card-3">
        <span class="icon"><NuxtImg src="/huhu.png" /></span>
        <p class="text">
          Mindfulify has truly transformed my digital experience. With <br />
          its user-friendly interface and comprehensive resources, I've<br />
          found solace and support in moments of stress. From guided<br />
          meditations to insightful articles, Mindfulify offers a holistic<br />
          approach to mental wellness that's both empowering and<br />
          uplifting. Highly recommend!
        </p>
        <span class="author">- Emily Smith, California</span>
      </div>
    </div>
  </div>
</template>


<script>

</script>

<style scoped>

.cards-section {
  width: 91%;
  background: #FFFAE5;
  max-width: 1355px;
  min-width: 290px;
  margin: 0 auto;
  padding: clamp(20px, 4vw, 60px);
  margin-top: -30px;
  min-height: clamp(300px, 50vw, 700px);
}

.cards-header {
  text-align: center;
  margin-bottom: clamp(10px, 2vw, 30px);
}

.cards-title {
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: clamp(25px, 3.5vw, 73px);
  color: #000;
}

.cards-container {
  position: relative; /* so absolutely positioned cards anchor here */
  min-height: clamp(300px, 50vw, 700px);
  min-width: 300px;
  margin-top: -20px;
}



.card {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  background: #FFFAE5;
  border-radius: clamp(4px, 1vw, 22px);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 10px;
  box-sizing: border-box;
}

/* Card 1 & 2 remain simple */
.card-1 {
  width: clamp(245px, 69vw, 1200px);
  top: clamp(38px, 2.6vw, 38px); /* slightly grows */
  z-index: 0;
  background: #FFFAE5;
  opacity: 0.165;
  border: 0.2px solid #000000;
}

.card-2 {
  width: clamp(280px, 75vw, 1250px);
  top: clamp(48px, 3.4vw, 54px); /* slightly grows */
  z-index: 1;
  background: #FFFAE5;
  opacity: 0.5;
  border: 0.29px solid #000000;
}

.card-3 {
  width: clamp(300px, 80vw, 1300px);
  top: clamp(60px, 4.5vw, 76px); /* slightly grows */
  z-index: 2;
  background: #FFFAE5;
  display: flex;
  flex-direction: column;
  border: 0.29px solid #000000;
}

.card-3 .icon {
  display: inline-block;
  width: clamp(20px, 6vw, 110px); /* Make it scale up */
   margin-top: clamp(0px, 1vw, 25px); /* Responsive top margin */
  margin-left: clamp(2px, 1.2vw, 40px); /* Responsive left margin */
  margin-bottom: clamp(8px, 2.7vw, 30px);
}

.card-3 .icon :deep(img) {
  width: 100%;
  height: auto;
  display: block;
  object-fit: contain;
}

.card-3 .text {
  flex-grow: 1;
  margin: 0;
  line-height: 1.5;
  margin-left: clamp(6px, 2.5vw, 70px);
  font-family: 'Outfit', sans-serif;
  font-size: clamp(9px, 2.5vw, 40px); /* Responsive scaling */
  font-weight: 200; /* Added to match your design system */
  letter-spacing: 0%; /* Explicitly set like your other components */
}
.card-3 .author {
  align-self: flex-end;
  color: #000000;
  margin-top: 7px;
  font-size: clamp(8px, 2vw, 30px);
  font-family: 'Outfit', sans-serif;
font-weight: 200;
line-height: 100%;
letter-spacing: 0%;
margin-bottom: clamp(0px, 0.5vw, 30px);
margin-right: clamp(10px, 1.5vw, 40px);
}
</style>