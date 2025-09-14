<template>
  <div class="foundation-wrapper">
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
        <img src="/group1.svg" alt="" />
      </div>
    </div>
    <!--  -->
    <div class="foundation-div2">
      <div class="image2">
        <img src="/group2.svg" alt="" />
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
  height: 230vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* padding-top: 50px; */
  padding-bottom: 50px;
}
.foundation-div {
  display: flex;
  align-items: center;
  justify-content: space-between;
  align-content: center;
  padding-left: 100px;
  padding-right: 100px;
  margin-bottom: 50px;
  height: 80vh;
}

.text {
  width: 50%;
  padding: 0;
}
.text h1 {
  font-size: 83px;
  font-family: 'Instrument Serif', serif;
  font-weight: 500;
  line-height: 1;
  color: #000000;
  margin-bottom: 10px;
}
.text p {
  font-size: 21px;
  font-weight: 400;
  line-height: 1.5;
  color: #000000;
  font-family: 'Montserrat', sans-serif;
}
.image1, .image2 {
  width: 50%;
  height: 90vh;
  display: flex;
  justify-content: left;
  align-items: center;
  padding: 0;

}
.image1{
  justify-content: right;
}
/*  */
.foundation-div2{
  display: flex;
  align-items: center;
  justify-content: space-between;
  align-content: center;
  padding-left: 100px;
  padding-right: 100px;
  margin-top: 66px;
  height: 90vh;
}

.foundation-div2 .text h1 {
  font-size: 78px;
  font-family: Impact;
  font-weight: 800;
  color: #000000;
  letter-spacing: 3px;
  margin-top: 30px;

}
.foundation-div2 .text{
  margin-top: 130px;
}
.foundation-div2 .text h2 {
  font-size: 66px;
 font-family: 'Instrument Serif', serif;
 font-style: italic;
  font-weight: 400;
  color: #000000;
  line-height: 1;
  margin: 0;
  width: 600px

}
</style>
