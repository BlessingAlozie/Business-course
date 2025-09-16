<template>
  <div class="container-wrapper">
    <div class="container">
      <h2>
        Early bird pricing ends in  <br><span>04 hours.</span> <b>REGISTER NOW TO save ₦10,000</b>
      </h2>
      <h1>03 : 53 : 40</h1>

       <button class="hvr-icon-forward">
        Join The Bootcamp &nbsp; &nbsp; &nbsp; &nbsp; <i class="fa-solid fa-arrow-right hvr-icon"></i>
      </button>
 </div>
  </div>
</template>

<script>

</script>

<style scoped>
.container-wrapper {
  width: 100%;
 font-family: 'Montserrat', sans-serif;
  background-color: #000000;
  text-align: center;
  align-content: center;
  padding-bottom: 50px;
}

.container {
  width: 100%;
  color: #ffffff;
  padding-top: 50px;
  padding-bottom: 50px;
  text-align: center;
}

.container h2 {
  font-size: 3rem;
  font-weight: 300;
  text-transform: uppercase;
  width: 62%;
  margin: auto;
  line-height: 3.5rem;
 text-align: center;
 padding-top: 50px;

}

.container h1 {
  font-size: 11.5rem;
  font-weight: 700;
  margin-top: 40px;
  color: #FF4124;


}

.container span {
  color: #FF4124;
  font-family: 'Montserrat', sans-serif;
  font-size: 4.1rem;
  font-weight: 700;
}

.container b{
  font-family: 'Montserrat', sans-serif;
   font-size: 4.1rem;
  font-weight: 700;
}

 button {
  /* margin-top: -30px; */
  background-color: #232323;
  color: white;
  border: none;
  padding: 30px 120px;
  font-size: 24px;
  font-family: "montserrat";
  font-weight: 600;
  cursor: pointer;

}

/* ✅ Responsive Styles */
@media (max-width: 1024px) {
  .container-wrapper {
    padding: 0 50px;
  }
  .container h2 {
    font-size: 3.5rem;
    line-height: 5rem;
    width: 90%;
  }
  .container h1 {
    font-size: 8rem;
  }
  .promise {
    max-width: 80%;
    padding: 40px 50px;
  }
}

@media (max-width: 768px) {
  .container-wrapper {
    padding: 0 20px;
  }
  .container {
    margin-top: 60px;
  }
  .container h2 {
    font-size: 2.2rem;
    line-height: 3.2rem;
    width: 100%;
  }
  .container h1 {
    font-size: 5rem;
    margin-top: 40px;
  }
  .promise {
    max-width: 100%;
    padding: 30px 20px;
  }
  .promise h3 {
    font-size: 1.8rem;
  }
  .promise p {
    font-size: 0.9rem;
  }
}

@media (max-width: 480px) {
  .container h2 {
    font-size: 1.6rem;
    line-height: 2.4rem;
  }
  .container h1 {
    font-size: 3.5rem;
    margin-top: 30px;
  }
  .promise {
    padding: 20px;
    border-radius: 20px;
  }
  .promise h3 {
    font-size: 1.5rem;
  }
  .promise p {
    font-size: 0.85rem;
    line-height: 1.5rem;
  }
}
</style>
