<template>
  <div class="hero-section">
    <div class="hero-texts">
      <h1>
        <span>TRANSFORM </span> YOUR BUSINESS IDEAS INTO
        <span>REALITY</span>
      </h1>
      <p>
        The complete step-by-step system that takes you from complete beginner
        to confident business owner with a fully operational business plan in
        Just 8 Weeks
      </p>
      <button class="hvr-icon-forward">
        Join The Bootcamp <i class="fa-solid fa-arrow-right hvr-icon"></i>
      </button>
    </div>

    <!-- ✅ Changed from background to real image -->
    <div class="hero-image">
      <img src="/hero-image.svg" alt="Hero Image" />
    </div>
  </div>
</template>

<style scoped>
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
  font-weight: 600;
  cursor: pointer;
}

/* ✅ Hero image styles */
.hero-image {
  display: flex;
  justify-content: center;
  align-items: center;
}
.hero-image img {
  width: 100%;
  height: 100%;
  object-fit: cover; 
}

/* Tablet */
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
    min-height: auto;
    width: 100%;
  }

  .hero-texts {
    padding: 0;
    text-align: center;
    order: 1;
  }

  .hero-image {
    order: 2;
    min-height: 350px;

  }


  .hero-texts h1 {
    font-size: 62px;
    line-height: 1.1;
  }
}

/* Small mobile */
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

  .hero-image img {
    max-height: 350px;
    width: 100%;
    object-fit: cover;
  }
}
</style>
