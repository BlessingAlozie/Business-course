<template>
  <div class="foundation-wrapper">
    <!-- Section 1 -->
    <div class="foundation-div">
      <div class="text">
        <h1>Building with <i>Systems</i> from ground-up</h1>
        <p>
          The structured step-by-step system that walks you from absolute beginner to confident
          business owner, equipping you with the skills, clarity, and systems to craft a solid
          business plan, validate your ideas, and launch a business you can proudly call your own.
        </p>
      </div>
      <div class="image1">
        <img src="/group1.svg" alt="Group 1" />
      </div>
    </div>

    <!-- Section 2 -->
    <div class="foundation-div2">
      <div class="image2">
        <img src="/group2.svg" alt="Group 2" />
      </div>
      <div class="text">
        <h1>MASTER THE FUNDAMENTALS</h1>
        <h2>Get It Right From Day One</h2>
        <p>
          Stop dreaming about starting your own business. This intensive 8-weeks masterclass gives you
          everything you need to validate your idea, build a rock-solid business plan,
          and launch successfully, even if you’re starting from scratch.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.foundation-wrapper {
  background-color: #ffffff;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-bottom: 50px;
  gap: 60px;
}

/* Shared text styles */
.text {
  width: 50%;
}
.text h1 {
  font-size: 83px;
  font-family: 'Instrument Serif', serif;
  font-weight: 500;
  line-height: 1.1;
  color: #000000;
  margin-bottom: 15px;
}
.text p {
  font-size: 21px;
  font-weight: 400;
  line-height: 1.6;
  color: #000000;
  font-family: 'Montserrat', sans-serif;
}

/* Images */
.image1, .image2 {
  width: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.image1 img, .image2 img {
  max-width: 100%;
  height: auto;
}

/* Section 1 */
.foundation-div {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 40px;
  padding: 0 100px;
}

/* Section 2 */
.foundation-div2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 40px;
  padding: 0 100px;
}

.foundation-div2 .text h1 {
  font-size: 78px;
  font-family: Impact;
  font-weight: 800;
  color: #000000;
  letter-spacing: 3px;
  margin-top: 20px;
}
.foundation-div2 .text {
  margin-top: 40px;
}
.foundation-div2 .text h2 {
  font-size: 66px;
  font-family: 'Instrument Serif', serif;
  font-style: italic;
  font-weight: 400;
  color: #000000;
  line-height: 1.1;
  margin: 0 0 20px 0;
  max-width: 600px;
}

/* ---------------- Responsive ---------------- */

/* Tablets */
@media (max-width: 1024px) {
  .text h1 {
    font-size: 50px;
  }
  .text p {
    font-size: 18px;
  }
  .foundation-div2 .text h1 {
    font-size: 52px;
  }
  .foundation-div2 .text h2 {
    font-size: 40px;
  }
  .foundation-div, .foundation-div2 {
    padding: 0 40px;
    gap: 20px;
  }
}

/* Mobile */
@media (max-width: 768px) {
  .foundation-div,
  .foundation-div2 {
    flex-direction: column;
    padding: 0 20px;
    text-align: center;
  }

  .text {
    width: 100%;
  }
  .text h1 {
    font-size: 32px;
  }
  .text p {
    font-size: 16px;
  }

  .foundation-div2 .text h1 {
    font-size: 36px;
    letter-spacing: 1px;
  }
  .foundation-div2 .text h2 {
    font-size: 28px;
    max-width: 100%;
  }

  .image1, .image2 {
    width: 100%;
    margin-top: 20px;
  }
}
</style>
