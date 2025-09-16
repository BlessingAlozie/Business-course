<template>
  <nav>
    <!-- Brand -->
    <div class="brand">
      <img src="/logo.svg" alt="Course Logo" />
    </div>

    <!-- Menu -->
    <div class="menu">
      <ul class="nav-links">
        <li><a href="#Curriculum" class="hvr-underline-from-center">Curriculum</a></li>
        <li><a href="#Testimonials" class="hvr-underline-from-center">Testimonials</a></li>
        <li><a href="#Pricing" class="hvr-underline-from-center">Pricing</a></li>
        <li><a href="#Contact" class="hvr-underline-from-center">Contact</a></li>
      </ul>

      <!-- CTA -->
      <a href=""><button class="cta-btn hvr-sweep-to-right">Enroll Now</button></a>
    </div>
  </nav>

  <HeroSection />
  <MainSection />
  <Foundation />
  <ImageSection />
  <Scale />
  <Syllabus />
  <!-- <Success /> -->
  <Testimonial />
  <Pricing />
  <Counter />
  <Form />
  <Footer />


</template>

<script>
import { RouterLink } from 'vue-router'
import HeroSection from './components/HeroSection.vue'
import MainSection from './components/MainSection.vue'
import Foundation from './components/Foundation.vue'
import ImageSection from './components/ImageSection.vue'
import Scale from './components/Scale.vue'
import Syllabus from './components/Syllabus.vue'
// import Success from './components/Success.vue'
import Testimonial from './components/Testimonial.vue'
import Pricing from './components/Pricing.vue'
import Counter from './components/Counter.vue'
import Form from './components/Form.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    HeroSection,
    MainSection,
    Foundation,
    ImageSection,
    Scale,
    Syllabus,
    // Success,
     Testimonial,
    Pricing,
    Counter,
    Form,
    Footer,


  },
}
</script>

<style>
html,
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
  overflow-x: hidden;
}
body {
  background-color: #fff7e4;
}
nav {
  background-color: #fff7e4;
  width: 100%;
  padding: 20px 100px;
  border-bottom: 1px solid #e0e0e0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0;
  box-sizing: border-box;
  align-content: center;
  font-family: 'Montserrat';
}

.brand img {
  width: 60px;
  height: 60px;
}

.menu {
  display: flex;
  align-items: center;
  gap: 2rem;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 2rem;
  margin: 0;
  padding: 0;
}

.nav-links li a {
  text-decoration: none;
  color: #333;
  font-weight: 600;
  font-size: 18px;
}

.cta-btn {
  color: white;
  padding: 0.9rem 1.3rem;
  cursor: pointer;
  font-weight: 600;
  border: 1px solid #000000;
  color: #000000;
  background-color: transparent;
  font-family: 'Montserrat';
  font-size: 18px;
  font-weight: 600;
}

.hvr-sweep-to-right:before {
  background: #ff4124 !important; /* custom sweep color */
  pointer-events: none !important; /* keep it clickable */
}

.cta-btn:hover {
  color: #fff;
  border-color: #ff4124;
}
.hvr-underline-from-center:before {
  background: #ff4124 !important;
  height: 3px; /* thickness */
}
</style>
