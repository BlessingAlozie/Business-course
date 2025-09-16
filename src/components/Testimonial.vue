<template>
  <!-- <div class="container">
    <div class="wrapper">
      <div class="text">
        <img src="/quote.png" alt="">
          <p>I went from just an idea to launching my marketing consultancy in 30 days. The step-by-step guidance made everything clear, and now I’m fully booked with clients and confident growing my business.</p>

          <b>Sarah Chibueze</b>
        <h6><small>Founder, Marketing Consultancy</small></h6>
      </div>
      <div class="image"></div>
    </div> -->
  <div class="splide container">
    <h1>What our students say about our program</h1>
    <div class="splide__track">
      <div class="splide__list">
         <!-- Move v-for to the slide level -->
        <div class="splide__slide wrapper" v-for="student in students" :key="student.name">
          <div class="text">
            <img :src="student.image" alt="" />
            <p>{{student.body}}</p>
            <b>{{student.name}}</b>
            <h6><small>{{student.profession}}</small></h6>
          </div>
          <div class="image" :style="{ backgroundImage: `url(${student.profileImage || '/sarah.jpg'})` }"></div>
        </div>
      </div>
    </div>
  </div>
  <!-- </div> -->
</template>

<script>
import { onMounted } from 'vue'
import Splide from '@splidejs/splide'
import { AutoScroll } from '@splidejs/splide-extension-auto-scroll'
import '@splidejs/splide/dist/css/splide.min.css'

export default {
  data() {
    return {
      students: [
        {
          name: 'Sarah Chibueze',
          profession: 'Founder, Marketing Consultancy',
          image: '/quote.png',
          profileImage: '/sarah.jpg',
          body: `I went from just an idea to launching my marketing consultancy in 30 days. The step-by-step guidance made everything clear, and now I'm fully booked with clients and confident growing my business.`,
        },
        {
          name: 'Chika Moses',
          profession: 'Founder, Tech Startup',
          image: '/quote.png',
          profileImage: '/smart-owner.svg',
          body: `The program transformed my approach to business. Within weeks, I had a clear roadmap and the confidence to execute. My startup is now generating consistent revenue.`,
        },
         {
          name: 'Jessica Uzochukwu',
          profession: 'E-commerce Entrepreneur',
          image: '/quote.png',
          profileImage: '/pink-woman.png',
          body: `From zero to six figures in 6 months. The strategies taught here are practical and results-driven. My online store is now my full-time income source.`,
        },
      ],
    }
  },
  mounted() {
    const splide = new Splide('.splide', {
      type: 'loop',
      drag: 'free',
      focus: 'center',
      perPage: 2,
      autoScroll: {
        speed: 1,
      },
    })
    splide.mount({ AutoScroll })
  },
}
</script>

<style scoped>
.container {
  height: 100vh;
  width: 100%;
  background-color: #fffcfc;
  text-align: center;
  align-items: center;
}
.container h1 {
  align-self: center;
  padding-bottom: 50px;
  padding-top: 50px;
  font-size: 3rem;
  font-weight: 300;
  font-family: 'Instrument Serif', serif;
  width: 400px;
  color: #000000;
  margin: auto;
  line-height: 0.9;
}

.wrapper {
  height: 400px;
  width: 50%;
  margin: 50px 20px;
  /* background-color: #900c7e; */
  border-radius: 8px;
  text-align: left;
  display: flex;
  border: 1px solid rgb(209, 209, 209);
}

.text,
.image {
  width: 50%;
  height: auto;
  background: #ffffff;
}
.text {
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
  padding: 30px;
}
.text p {
  font-size: 18px;
  font-weight: 400;
  font-family: 'montserrat';
  padding-bottom: 50px;
  line-height: 1.7rem;
}
.image {
  /* background-image: url('/sarah.jpg'); */
  background-size: cover;
  background-repeat: no-repeat;
  background-position: right center;
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
}
.text b {
  padding-bottom: 10px;
}
.text h6 {
  margin: 0;
  padding: 0;
  font-size: 14px;
  font-weight: 400;
}



/* Adding custom pagination dot styles */
/* :deep(.splide__pagination) {
  bottom: -40px;
} */

:deep(.splide__pagination__page) {
  background: #d1d1d1;
  opacity: 0.7;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  transition: all 0.3s ease;
}

:deep(.splide__pagination__page.is-active) {
  background: #ff4124;
  opacity: 1;
  transform: scale(1.2);
}

:deep(.splide__pagination__page:hover) {
  background: #ff4124;
  opacity: 0.8;
}
</style>
