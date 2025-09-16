<template>
  <footer class="footer">
    <div class="footer-left">
      <!-- Social Media Links -->
      <div class="social-links">
        <a href="https://instagram.com/themomshub_" target="_blank" aria-label="Instagram">
          <i class="fab fa-instagram"></i>
        </a>
        <a href="https://twitter.com/The_Moms_HuB" target="_blank" aria-label="Twitter">
         <i class="fa-brands fa-x-twitter"></i>
        </a>
        <a href="https://linkedin.com/company/the-moms-hub" target="_blank" aria-label="LinkedIn">
          <i class="fab fa-linkedin"></i>
        </a>
        <a href="https://facebook.com/TheMomsHub" target="_blank" aria-label="Facebook">
          <i class="fab fa-facebook"></i>
        </a>
      </div>

      <!-- Contact Info -->
      <div class="contact-info">
         GET IN TOUCH : <a href="mailto:info@themumshub.com">info@themumshub.com</a>
      </div>

      <!-- Brand Logo -->
      <div class="brand-section">
        <div class="logo">
          <img src="/logo.svg" alt="" />
        </div>
        <div class="brand-text">THE MOM'S HUB © 2025</div>
      </div>
    </div>

    <div class="footer-right">
      <div class="back-to-top" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
        <span class="arrow-up"><img src="/arrow-up.svg" alt="" /></span>
        BACK TO TOP
      </div>
      <div class="phone-number">+234 816 000 6890</div>
      <div class="address">375 HERBERT MACAULAY WAY, YABA, LAGOS</div>
    </div>
  </footer>

  <LiveClasses />
</template>

<script>
import LiveClasses from '@/components/LiveClasses.vue'

export default {
  components: {
    LiveClasses,
  },
}
</script>

<style scoped>
.footer {
  color: #000000;
  padding-left: 100px;
  padding-right: 100px;
  padding-top: 150px;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  min-height: 150px;
  margin-bottom: -40px;
  background-color: #ffffff;
  padding-bottom: 80px;
  font-family: "montserrat";
}

.footer-left {
  display: flex;
  flex-direction: column;
  gap: 20px;
  font-family: "montserrat";
}

/* 🔥 Social Media Styling */
.social-links {
  display: flex;
  gap: 15px;
  font-size: 1.5rem;
  font-family: "montserrat";
}

.social-links a {
  color: rgb(6, 6, 6);
  transition: color 0.3s ease;
  font-family: "montserrat";
}

.social-links a:hover {
  color: #FF4124; /* Light green hover */
}

.contact-info {
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 0.5px;
  font-family: "montserrat";
}

.contact-info a {
  color: rgb(0, 0, 0);
  /* text-decoration: none; */
  font-family: "montserrat";
}

.contact-info a:hover {
  text-decoration: underline;
  font-family: "montserrat";
}

.brand-section {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-top: 20px;
  font-family: "montserrat";
}

.logo {
  width: 60px;
  height: 60px;
  background-color: rgb(0, 0, 0);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: black;
  font-weight: bold;
  font-size: 10px;
  text-align: center;
  line-height: 1.1;
}

.brand-text {
  font-size: 18px;
  font-weight: bold;
  letter-spacing: 1px;
  font-family: "montserrat";
}

.footer-right {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 20px;
  width: 40%;
  text-align: right;
  font-family: "montserrat";
}

.back-to-top {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 1px;
  cursor: pointer;
  transition: opacity 0.3s ease;
  font-family: "montserrat";
}

.back-to-top:hover {
  opacity: 0.8;
}

.arrow-up {
  font-size: 20px;

}

.phone-number {
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 0.5px;
  font-family: "montserrat";
}

.address {
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 0.5px;
  line-height: 1.3;
  font-family: "montserrat";
}

@media (max-width: 768px) {
  .footer {
    flex-direction: column;
    gap: 30px;
    padding: 30px 40px;

  }

  .footer-right {
    align-items: flex-start;
    text-align: left;
    width: 100%;
  }

  .back-to-top {
    align-self: flex-start;
  }

  .social-links {
    justify-content: flex-start;
  }
}

@media (max-width: 768px) {

}
</style>
