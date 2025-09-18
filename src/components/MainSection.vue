<template>
  <div class="main-section">
    <h1>
      <span>LEARN THE SECRETS TO <strong>STARTING</strong> A </span>SMALL BUSINESS IN AFRICA
    </h1>

    <div class="smart-owner">
      <!-- Left Image -->
      <div class="smart-image">
        <img src="/smart-owner.svg" alt="Smart Owner" />
      </div>

      <!-- Middle Text -->
      <div class="smart-text">
        <h2>
          <span>GOING FROM A </span>STRUGGLING <span>BUSINESS OWNER</span> TO A
        </h2>
        <h1>SMART FOUNDER</h1>
        <p>Join 200+ business women in Africa today...</p>
      </div>

      <!-- Right Image -->
      <div class="founder2">
        <img src="/founder2.svg" alt="Founder" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.main-section {
  height: auto;
  padding: 0 20px;
  background-color: #000000;
  color: #ffffff;
  align-content: center;
  padding-left: 100px;
  padding-right: 100px;
}

.main-section h1 {
  font-size: 118px;
  font-family: 'Poppins', sans-serif;
  font-weight: 800;
  line-height: 1;
  text-align: left;
}

.main-section h1 span {
  color: #b6b6b6;
}

.main-section h1 span strong {
  color: #787878;
}

.smart-owner {
  display: flex;
  align-items: center;
  margin-top: 50px;
  margin-bottom: 70px;
}

/* Image Containers */
.smart-image,
.founder2 {
  height: 600px;
  background-color: #FF4124;
  display: flex;
  align-items: center;
  justify-content: center;
}

.smart-image {
  width: 35%;
}

.founder2 {
  width: 25%;
}

/* Images */
.smart-image img,
.founder2 img {
  width: 100%;
  height: 100%;
  object-fit: cover;  /* fill div */
  object-position: center;
}

/* Text Section */
.smart-text {
  background-color: #FF4124;
  width: 40%;
  height: 600px;
  padding-left: 36px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.smart-text h2 {
  font-size: 50px;
  font-family: 'Bebas Neue', sans-serif;
  font-weight: 800;
  color: #ffffff;
  margin: 0;
  line-height: 1;
  width: 400px;
  word-spacing: 4px;
  padding-left: 30px;
}

.smart-text h1 {
  font-size: 161.94px;
  font-family: 'Bebas Neue', sans-serif;
  font-weight: 800;
  width: 400px;
  color: #ffffff;
  margin: 0;
  padding-left: 30px;
}

.smart-text p {
  font-size: 33px;
  font-weight: 400;
  color: #f1e0e0;
  margin: 0;
  padding-left: 30px;
  padding-top: 20px;
  font-family: 'Bebas Neue', sans-serif;
}

.smart-text span {
  color: #fcaeae;
}

/* ---------------- Responsive ---------------- */

/* Tablets */
@media (max-width: 1249px) {
  .main-section {
    margin-top: 50px;
  }
  .main-section h1 {
    font-size: 115px;
  }
  .smart-text {
    padding-left: 10px;
  }
  .smart-text h1 {
    font-size: 160px;
  }
  .smart-text p {
    padding-top: 0px;
  }
}

@media (max-width: 1024px) {
  .main-section {
    margin-top: 30px;
  }
  .main-section h1 {
    font-size: 60px;
  }
  .smart-text {
    width: 60%;
    height: 600px;
  }
  .smart-text h2 {
    font-size: 50px;
    width: auto;
    padding-left: 20px;
  }
  .smart-text h1 {
    font-size: 161.94px;
    width: auto;
    padding-left: 20px;
  }
  .smart-text p {
    font-size: 20px;
    padding-left: 20px;
  }
  .founder2 {
    display: none;
  }
}

/* Mobile */
@media (max-width: 968px) {
  .main-section {
    padding-left: 20px;
    padding-right: 20px;
  }
  .main-section h1 {
    font-size: 80px;
    text-align: left;
  }
  .smart-owner {
    flex-direction: column;
    padding: 0px;
  }
  .smart-image {
    height: 500px;
    width: 100%;
    background-color: transparent;
  }
  .smart-text {
    height: auto;
    padding: 20px;
    text-align: left;
    width: 95.6%;
  }
  .smart-text h2 {
    font-size: 40px;
    padding-bottom: 20px;
  }
  .smart-text h1 {
    padding-bottom: 20px;
  }
  .smart-text h2,
  .smart-text h1,
  .smart-text p {
    width: auto;
    padding-left: 0;
  }
  .founder2 {
    display: none;
  }
}

@media (max-width: 768px) {
  .main-section h1 {
    font-size: 60px;
  }
}

@media (max-width: 480px) {
  .main-section h1 {
    font-size: 50px;
  }
}
</style>
