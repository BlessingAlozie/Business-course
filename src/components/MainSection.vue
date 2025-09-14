<template>
  <div class="main-section">
    <h1>
      <span>LEARN THE SECRETS TO <strong>STARTING</strong> A </span>SMALL BUSINESS IN AFRICA
    </h1>
    <div class="smart-owner">
      <div class="smart-image">
        <!-- <img src="/smart-owner.svg" alt="Smart Owner" /> -->
      </div>
      <div class="smart-text">
        <h2> <span>GOING FROM A </span>STRUGGLING <span>BUSINESS OWNER</span> TO A</h2>
        <h1>SMART FOUNDER</h1>
        <p>Join 200+ business women in Africa today...</p>
      </div>
      <div class="founder2">
        <!-- <img src="/founder2.svg" alt=""> -->
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
  line-height: 1;
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

.smart-image {
  background-image: url('./smart-owner.svg');
  background-color: #FF4124;
  background-size: cover;
  background-repeat: no-repeat;
  object-fit: cover;
  background-position:  center;
  width: 35%;
  height: 600px;
}

.smart-text {
  background-color: #FF4124;
  width: 40%;
  height: 600px;
  padding-left: 36px;
}
.smart-text h2 {
  font-size: 50px;
  font-family: 'Bebas Neue', sans-serif;
  font-weight: 800;
  color: #ffffff;
  margin: 0;
  padding-top: 50px;
  line-height: 1;
  width: 400px;
  padding-left: 30px;
  word-spacing: 4px;
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
.founder2 {
  background-image: url('./founder2.svg');
  background-size: contain;
  background-repeat: no-repeat;
  object-fit: contain;
  background-position:  right;
  width: 25%;
  height: 600px;
  background-color: #FF4124;

}
</style>
