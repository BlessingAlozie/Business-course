<template>
  <div class="hero-section">
    <div class="hero-texts">
      <h1><span>TRANSFORM </span> YOUR BUSINESS IDEAS INTO <span>REALITY</span></h1>
      <p>
        The complete step-by-step system that takes you from complete beginner to confident business
        owner with a fully operational business plan in Just 8 Weeks
      </p>
      <button class="hvr-icon-forward">
        Join The Bootcamp <i class="fa-solid fa-arrow-right hvr-icon"></i>
      </button>
    </div>
    <div class="hero-image">
    </div>
  </div>
</template>

<script></script>

<style scoped>
html,
body {
  margin: 0;
  padding: 0;
    box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
}

.hero-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 100px;
    min-height: 80vh;
  max-width: 100vw;
}
.hero-texts, .hero-image {
    flex: 1;
   min-height: 80vh;


}
.hero-texts{
 align-content: center;
  padding: 30px 100px 0 0;
}
.hero-texts h1{
  font-size: 78px;
  font-family: Impact;
  font-weight: 800;
  color: #000000;
  letter-spacing: 3px;
  margin: 0;

}
.hero-texts h1 span {
  color: #FF4124;
}
.hero-image {
  background-image: url('./hero-image.svg');
  background-size: cover;
  background-repeat: no-repeat;
  object-fit: cover;
  background-position:  left;
  background-color: #615252;
}
.hero-texts p {
  font-size: 20px;
  font-family: "montserrat";
  font-weight: 400;
  color: #000000;
  line-height: 1.5;
}
.hero-texts button {
  margin-top: 30px;
  background-color: #000000;
  color: white;
  border: none;
  padding: 20px 30px;
  font-size: 18px;
  font-family: "montserrat";
  font-weight: 600;
  cursor: pointer;
}
</style>
