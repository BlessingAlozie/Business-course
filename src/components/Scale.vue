<template>
<div class="scale-section">
  <div class="texts">
    <h1>LEARN! GROW!! SCALE!!!</h1>
  </div>
  <div class="image">
    <img src="/pink-woman.png" alt=""></img>
  </div>
  </div>
  <div class="difference">
     <div class="text-left">
      <h1>This program gives you everything in one place</h1>
      <p>From legal setup to marketing, It is designed for beginners to confidently build their business plan as they learn.
         You’ll get expert guidance through weekly sessions, ongoing mentorship, and lifetime access to a supportive  community.
         Trusted by over 500 successful graduates, it’s a proven system that equips you to launch your business.</p>
    </div>
    <div class="text-right">
      <h1>What Makes This Different</h1>
    </div>
  </div>

</template>

<style scoped>
.scale-section{
  height: auto;
  padding-left: 100px;
  padding-right: 100px;
  color: #000000;
  display: flex;
gap: 168px;
text-align: center;
}
.scale-section h1{
  font-size: 185px;
  font-family: Impact;
  font-weight: 600;
  color: #000000;
  width: 400px;
  margin: 0;
  line-height: 0.9;
  padding-top: 200px;
  letter-spacing: 10px;
}
.difference{
  width: 87%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 550px;
  background-color: #ffffff;
  margin-top: -10px;
  margin-bottom: 70px;

}
.text-left{
  width: 50%;
  height: 480px;
  /* background-color: #fff; */
  padding: 50px;
 align-items: center;
}
.text-left h1{
  font-size: 84px;
  font-family: 'Instrument Serif', serif;
  font-weight: 550;
  line-height: 1;
  color: #000000;
  margin-top: 0;
  margin-bottom: 20px;
}
.text-left p{
  font-size: 21px;
  font-weight: 400;
  line-height: 1.5;
  color: #000000;
  font-family: 'Montserrat', sans-serif;
}


.text-right{
 width: 50%;
  height: 550px;
  background-color: #DF014A;
    text-align: center;
  align-content: center;
}
.text-right h1{
  font-size: 100px;
  font-family: 'Instrument Serif', serif;
  font-weight: 500;
  line-height: 1;
  color: #ffffff;
  padding: 50px;
  margin-top: 80px;
  margin-bottom: 20px;
}

@media (max-width: 768px) {
  .scale-section {
    flex-direction: column;
    padding-left: 20px;
    padding-right: 20px;
    gap: 40px;
    text-align: center;
  }

  .scale-section h1 {
    font-size: 84px;
    width: auto;
    padding-top: 80px;
    letter-spacing: 4px;
  }

  .image img {
    width: 100%;
    height: 400px;
    object-fit: contain;
  }

  .difference {
    flex-direction: column;
    height: auto;
    margin-top: 20px;
    margin-bottom: 40px;
  }
   .text-left{
    background-color: #ffffff;
    padding: 0px;
   }
   .text-right{
    order: -1;
   }

  .text-left, .text-right {
    width: 100%;
    height: auto;
    padding: 20px;
  }
.text-left h1 {
    font-size: 36px;
    margin-bottom: 10px;
  }

  .text-left p {
    font-size: 16px;
  }

  .text-right h1 {
    font-size: 40px;
    padding: 20px;
    margin-top: 40px;
  }
}


</style>
