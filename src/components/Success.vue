<template>
  <div class="containerr">
    <div class="text">
      <div class="h2">
        <h2>EVERYHING YOU NEED FOR</h2>
      </div>
      <div class="h1">
        <h1><span>BUSINESS</span><br  class="break"/> SUCCESS</h1>
      </div>
    </div>
    <div class="image">
      <img src="/sucess-b.svg" alt="" />
    </div>
  </div>
</template>

<style>
.containerr {
  max-width: 100%;
  height: auto;
  padding: 0 100px 100px;
  overflow-x: hidden;
  background-color: #000000;
}

.containerr .text {
  color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 2rem;
}

.h1 {
  margin: 0;
  line-height: 1;
  width: 60%;
}

.h1 h1 {
  font-size: 8rem;
  font-weight: 900;
  font-family: 'montserrat';
}

.h1 h1 span {
  color: #ff4124;
}

.h2 {
  margin: 0;
  line-height: 1;
  width: 40%;
  align-content: center;
}

.text h2 {
  font-size: 5rem;
  font-weight: 400;
  margin: 0;
  line-height: 1;
  font-family: 'Instrument Serif', serif;
}

.image img {
  max-width: 100%;
  height: auto;
  display: block;
  margin: 2rem auto 0;
}

/* 📱 Tablets */
@media (max-width: 1024px) {
  .containerr {
    padding: 0 50px 80px;
  }

  .h1 h1 {
    font-size: 5rem;
  }

  .text h2 {
    font-size: 3rem;
  }
}

/* 📱 Mobile */
@media (max-width: 768px) {
  .containerr .text {
    flex-direction: column;
    text-align: center;
  }

  .h1,
  .h2 {
    width: 100%;

  }

  .h1 h1 {
    font-size: 3rem;
    margin: 0;
  }

  .text h2 {
    font-size: 2rem;
     margin-top: 50px;
  }
  .break{
    display: none;
  }
}

/* 📱 Small Mobile */
@media (max-width: 480px) {
  .containerr {
    padding: 0 20px 60px;
  }

  .h1 h1 {
    font-size: 2.2rem;
  }

  .text h2 {
    font-size: 1.5rem;
  }
}


</style>
