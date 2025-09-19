<template>
  <nav>
    <div class="brand">
      <img src="/logo.svg" alt="Course Logo" />
    </div>

    <!-- Hamburger (for mobile) -->
    <button class="hamburger" @click="toggleMenu">
      <i v-if="!isOpen" class="fa-solid fa-bars"></i>
      <i v-else class="fa-solid fa-xmark"></i>
    </button>

    <div class="menu" :class="{ show: isOpen }">
      <ul class="nav-links">
        <li><a href="#Syllabus" class="hvr-underline-from-center">Curriculum</a></li>
        <li><a href="#Testimonials" class="hvr-underline-from-center">Testimonials</a></li>
        <li><a href="#Pricing" class="hvr-underline-from-center">Pricing</a></li>
        <li><a href="#Footer" class="hvr-underline-from-center">Contact</a></li>
      </ul>

      <button class="cta-btn hvr-sweep-to-right" @click="showModal = true">Enroll Now</button> v
    </div>
  </nav>
  <Signup :showModal="showModal" @close="showModal = false" />

  <HeroSection />
  <MainSection />
  <Foundation />
  <ImageSection />
  <Scale />
  <Syllabus />
  <Success />
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
import Success from './components/Success.vue'
import Testimonial from './components/Testimonial.vue'
import Pricing from './components/Pricing.vue'
import Counter from './components/Counter.vue'
import Form from './components/Form.vue'
import Footer from './components/Footer.vue'
import Signup from './components/Signup.vue'

export default {
  name: 'App',
  components: {
    HeroSection,
    MainSection,
    Foundation,
    ImageSection,
    Scale,
    Syllabus,
    Success,
    Testimonial,
    Pricing,
    Counter,
    Form,
    Footer,
    Signup,
  },

  data() {
    return {
      isOpen: false,
      showModal: false,
    }
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen
    },
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
  position: fixed;
  z-index: 9999;
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
  background: #ff4124 !important;
  pointer-events: none !important;
}

.cta-btn:hover {
  color: #fff;
  border-color: #ff4124;
}
.hvr-underline-from-center:before {
  background: #ff4124 !important;
  height: 3px;
}
.hamburger {
  display: none;
}
/* mobile responsiveness */
@media (max-width: 968px) {
  nav {
    padding-left: 30px;
    padding-right: 30px;
  }
  .menu {
    display: none;
    flex-direction: column;
    justify-content: center; /* centers links vertically */
    align-items: center;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    background-color: #fff7e4;
    z-index: 999;
  }

  .nav-links {
    flex-direction: column;
    align-items: center;
    gap: 1rem;
    margin: 0;
    padding: 0;
  }
  .nav-links li {
    width: 100%;
  }

  .nav-links li a {
    display: block;
    width: 100%;
    padding: 8px 0;
  }

  .menu.show {
    display: flex;
  }
  .hamburger {
    display: block;
    font-size: 28px;
    background: none;
    border: none;
    cursor: pointer;
    position: absolute;
    top: 25px;
    right: 30px;
    z-index: 1000;
  }
}

/* Desktop view */
/* @media (min-width: 1000px) {
  .hamburger {
    display: none;
  }

  .menu {
    display: flex;
    position: static;
    background: none;
    border: none;
    flex-direction: row;
  }
  .nav-links {
    flex-direction: row;
    align-items: center;
  }
} */
</style>
