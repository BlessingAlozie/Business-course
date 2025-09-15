<template>
  <div class="container">
    <div class="text">
      <div class="h2">
        <h2>EVERYHING YOU NEED FOR</h2>
      </div>
      <div class="h1">
        <h1><span>BUSINESS</span><br />SUCCESS</h1>
      </div>
    </div>
    <div class="image">
      <img src="/sucess-b.svg" alt="" />
    </div>
  </div>
</template>

<style>
.container {
  max-width: 90%;
  min-height: 100vh;
  padding-left: 100px;
  padding-right: 100px;
  overflow-x: hidden;
  background-color: #000000;
  padding-bottom: 100px;
}

.text {
  color: #fff;
  padding-top: 100px;
  overflow-x: hidden;
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
  /* font-family: 'montserrat'; */
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
.image {
  background-color: #e15858;
  height: 600px;
}
.image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
