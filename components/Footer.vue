<template>
  <footer class="footer-wrapper">
    <div class="footer-content">

      <div class="footer-row">
  <!-- Logo Section -->
  <div class="footer-brand">
    <img src="/LOGO02.png" alt="Logo" class="logo-img" />
    <p class="footer-description">
      Your go-to destination for embracing mindfulness
      and finding inner peace midst the digital noise of today's world.
    </p>
  </div>

  <!-- Footer Columns -->
  <div class="footer-columns">
    <div class="footer-column">
      <h4 class="mini-title">Quick Menu</h4>
      <ul class="column-list">
        <li>About</li>
        <li>Pricing</li>
        <li>Blog</li>
        <li>Help</li>
      </ul>
    </div>
    <div class="footer-column">
      <h4 class="mini-title">Resources</h4>
      <ul class="column-list">
        <li>Newsletter</li>
        <li>Community</li>
        <li>Jobs</li>
        <li>Forums</li>
      </ul>
    </div>
  </div>

  <!-- Subscribe Section -->
  <div class="footer-subscribe">
    <h4 class="subscribe-title">Subscribe to our newletter</h4>
    <p class="subscribe-text">Subscribe now to be updates with the latest features</p>
    <div class="subscribe-form">
      <input type="email" placeholder="Your email address" />
      <button class="hidden-button">Subscribe</button>
    </div>
  </div>
</div>




      <!-- Bottom Bar -->
      <div class="footer-bottom">
        <p class="rights-text">@2024 Mindfulify All Rights Reserved</p>
        <div class="social-icons">
          <a href=""><img src="/FFF.png" alt="Facebook" class="face"  /></a>
          <a href=""><img src="/III.png" alt="Twitter" /></a>
          <a href=""><img src="/TTT.png" alt="Instagram" /></a>
        </div>
      </div>

    </div>
  </footer>
</template>


<style scoped>


.footer-row {
  display: flex;
  flex-direction: column;
  gap: clamp(20px, 4vw, 40px);
}

.footer-subscribe{
    display: none;
}

.footer-wrapper {
  background: #FFFAE5;
  color: #fff;
  padding: clamp(30px, 5vw, 60px) clamp(20px, 4vw, 50px);
  min-width: 290px;
  max-width: 1375px;
  margin: 0 auto;
}

.footer-content {
  background-color: #000;
  max-width: 1270px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  gap: clamp(30px, 5vw, 60px);
  padding: 20px;
  border-radius: 14px;
}

.footer-top {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: clamp(20px, 5vw, 40px);
  
}

.footer-brand {
  text-align: left;
  flex: 1 1 100%;
}


.footer-columns {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
  gap:0px; 
}

.footer-column {
  flex: 1 1 150px;
  min-width: 100px;
  margin-right: -50px;
}



.logo-img {
  width: clamp(80px, 15vw, 140px);
  height: auto;
  zoom: 1.8;
}

.footer-description {
  font-size: clamp(12px, 1.5vw, 18px);
  line-height: 1.6;
  color: #ffffff;
  font-family: 'Outfit';
font-weight: 300;
line-height: 120%;
letter-spacing: 0%;
margin-bottom: -23px;
}

.mini-title {
  font-size: clamp(14px, 2vw, 20px);
  margin-bottom: clamp(12px, 1.5vw, 16px);
  font-weight: 600;
  color: #fff;
  font-family: 'Outfit';
font-weight: 300;
line-height: 100%;
letter-spacing: 0%;
}

.column-list {
  list-style: none;
  padding: 0;
  margin: 0;

}

.column-list li {
  font-size: clamp(13px, 1.4vw, 16px);
  margin-bottom: 12px;
  color: #aaa;
  font-family: 'Outfit';
font-weight: 200;
line-height: 100%;
letter-spacing: 0%;

}

.footer-bottom {
  border-top: 1px solid #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  padding-top: clamp(12px, 2vw, 20px);
  gap: 20px;
  margin-bottom: 10px;
}

.rights-text {
  font-size: clamp(10px, 1.3vw, 16px);
  color: #bbb;
  font-family: 'Outfit';
font-weight: 400;
line-height: 100%;
letter-spacing: 0%;

}

.social-icons {
  display: flex;
  align-items: center;   /* vertically center icons */
  gap: clamp(5px, 1.5vw, 10px);  /* better than margin-left for spacing */
}

.social-icons a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: clamp(18px, 4vw, 30px);
  height: clamp(18px, 4vw, 30px);
  border: 0.4px solid #FFFFFF;
  border-radius: 50%;
  background-color: transparent;
  transition: transform 0.3s ease;
}

.social-icons img {
  width: 75%;
  height: auto;
  display: block;
}

.social-icons img.face {
  width: 50%;
}




@media (min-width: 1250px) {
  .footer-row {
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    gap: clamp(10px, 2vw, 20px);
  }

  .footer-brand {
    flex: 1 1 30%;
    margin-top: 25px;
    margin-left: 25px;
    max-width: 300px;
  }

  .footer-columns {
    flex: 1 1 30%;
    display: flex;
    flex-direction: row;
    gap: -20px; 
    text-align: right;
    margin-right: 90px;
    margin-left: -40px;
  }

  .footer-subscribe {
    flex: 1 1 30%;
  }
.footer-subscribe {
  display: flex;
  flex-direction: column;
  gap: clamp(10px, 1vw, 20px);
  max-width: 350px;
  margin-right: 30px;

}


.hidden-button {
  display: block !important;
}
.column-list{
    text-align: right;
}

}



.subscribe-title {
  font-size: clamp(14px, 2vw, 20px);
  font-weight: 600;
  color: #fff;
  font-family: 'Outfit';
font-weight: 400;
line-height: 100%;
letter-spacing: 0%;
margin-bottom: -15px;
}

.subscribe-text {
  font-size: clamp(8px, 1vw, 12px);
  max-width: 250px;
  color: #ffffff;
  font-family: 'Outfit';
font-weight: 100;
line-height: 110%;
letter-spacing: 0%;
margin-bottom: 0px;
}

.subscribe-form {
  display: flex;
  flex-direction: column;
  position: relative;
}

.subscribe-form input[type="email"] {
  padding: clamp(20px, 1.5vw, 14px);
  font-size: clamp(12px, 1.4vw, 16px);
  border: 1px solid #ccc;
  border-radius: 28px;
  background-color: #fff;
  color: #000;
  box-shadow: 0px 9.61px 0px 0px #000000;
}

.hidden-button {
  position: absolute;
  top: 50%;
  right: 10px;
  transform: translateY(-50%);
  display: none; /* Will be shown via media query */
  padding: 14px 14px;
  background: #FBC56F;
  color: #000;
  border: 1px solid #ccc;
  border-radius: 18px;
  cursor: pointer;
  font-family: 'Outfit';
  font-weight: 500;
  line-height: 100%;
  text-align: center;
  font-size: clamp(12px, 1.4vw, 16px);
  font-family: 'Outfit';
font-weight: 500;
line-height: 100%;
letter-spacing: 0%;
text-align: center;


}

</style>
