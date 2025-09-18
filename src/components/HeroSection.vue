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
    <div class="hero-image"></div>
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

.hero-texts,
.hero-image {
  flex: 1;
  min-height: 80vh;
}

.hero-texts {
  align-content: center;
  padding: 30px 100px 0 0;
}

.hero-texts h1 {
  font-size: 78px;
  font-family: Impact;
  font-weight: 800;
  color: #000000;
  letter-spacing: 3px;
  margin: 0;
}

.hero-texts h1 span {
  color: #ff4124;
}

.hero-image {
  background-image: url('./hero-image.svg');
  background-size: cover;
  background-repeat: no-repeat;
  object-fit: cover;
  background-position: left;
  border-left-color: #000000;
  min-height: 80vh;
}

.hero-texts p {
  font-size: 20px;
  font-family: 'montserrat';
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
  font-family: 'montserrat';
  font-weight: 600;
  cursor: pointer;
}

/* Tablet styles */
/* @media (max-width: 1024px) {
  .hero-section {
    padding: 0 100px;
  }

  .hero-texts {
    padding: 30px 50px 0 0;
  }

  .hero-texts h1 {
    font-size: 70px;
    letter-spacing: 2px;
  }

  .hero-texts p {
    font-size: 18px;
  }

  .hero-texts button {
    font-size: 16px;
    padding: 18px 25px;
  }
} *
/* Mobile styles */
@media (max-width: 968px) {
  .hero-section {
    flex-direction: column;
    padding: 20px;
    min-height: 100vh;
    gap: 30px;
  }

  .hero-texts,
  .hero-image {
    flex: none;
    min-height: 350px;
    width: 100%;
  }

  .hero-texts {
    padding: 0;
    text-align: center;
    order: 1;
    width: 100%;
  }

  .hero-image {
    order: 2;
    min-height: 550px;
    width: 100%;
    background-position: center;
  }

  .hero-texts h1 {
    font-size: 62px;
    letter-spacing: 1px;
    line-height: 1.1;
  }

  .hero-texts p {
    font-size: 16px;
    margin: 20px 0;
  }

  .hero-texts button {
    font-size: 16px;
    padding: 15px 25px;
    margin-top: 20px;
  }
}
/* Small mobile styles */
@media (max-width: 480px) {
  .hero-section {
    padding: 15px;
    gap: 20px;
  }

  .hero-texts h1 {
    font-size: 32px;
    letter-spacing: 0.5px;
  }

  .hero-texts p {
    font-size: 14px;
  }

  .hero-texts button {
    font-size: 14px;
    padding: 12px 20px;
    width: 100%;
    max-width: 280px;
  }

  .hero-image {
    min-height: 350px;
  }
}
</style>
