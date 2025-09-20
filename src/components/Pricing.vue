<template>
  <section class="pricing-section" id="Pricing">
    <h2>Our <i>Flexible</i> Pricing Plans</h2>
    <p>Choose the track that best fits your journey to becoming a successful Virtual Assistant.</p>

    <div class="pricing-cards">
      <!-- Card 1 -->
      <div class="card card1">
        <h3>Essential Track</h3>
        <div class="price">₦50,000</div>
        <ul>
          <li>Core Virtual Assistant Training</li>
          <li>Access to Mom’s Support Community</li>
        </ul>
        <button class="btn">Get Started</button>
      </div>

      <!-- Card 2 (highlighted) -->
      <div class="card highlight">
        <div class="most-popular">Most Popular</div>
        <div class="contents">
          <h3>Professional Track</h3>
          <div class="price">₦100,000</div>
          <ul>
            <li>Core Virtual Assistant Training</li>
            <li>Access to Mom’s Support Community</li>
            <li>1-on-1 Mentoring Sessions</li>
            <li>Client Template Library</li>
          </ul>
          <button class="btn highButton">Get Started</button>
        </div>
      </div>

      <!-- Card 3 -->
      <div class="card card3">
        <h3>VIP Accelerator</h3>
        <div class="price">₦200,000</div>
        <ul>
          <li>Core Virtual Assistant Training</li>
          <li>Access to Mom’s Support Community</li>
          <li>Core Virtual Assistant Training</li>
          <li>Access to Mom’s Support Community</li>
          <li>Core Virtual Assistant Training</li>
          <li>Access to Mom’s Support Community</li>
        </ul>
        <button class="btn">Get Started</button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.pricing-section {
  width: 100%;
  margin: auto;
  text-align: center;
  padding: 50px 0px;
  background-color: #fff;
  padding-bottom: 100px;
}

.pricing-section h2 {
  color: #000000;
  font-size: 3rem;
  font-weight: 600;
  margin-bottom: 10px;
  font-family: 'Instrument Serif', serif;
}

.pricing-section p {
  color: #000000;
  max-width: 415px;
  margin: 0 auto 50px;
  font-size: 0.9rem;
}

.pricing-cards {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 150px;
}

.card {
  background-color: #ffffff;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: left;
  min-height: 400px;
  width: 392px;
  position: relative;
  padding-top: 20px;
  padding-bottom: 60px;
  box-shadow: 0px 8px 8px 2px rgba(0, 0, 0, 0.15);
}

.card1,
.card3 {
  padding-left: 20px;
  padding-right: 20px;
}
.highlight {
  /* border: 1px solid #000000; */
  position: relative;
  background-color: #ffffff;
  min-height: 438px;
  margin-top: -45px;
}

.most-popular {
  background-color: #ffc2b9;
  height: 50px;
  position: relative;
  width: 100%;
  color: #ff4124;
  margin: -30px;
  border-top-right-radius: 12px;
  border-top-left-radius: 12px;
  font-size: 1.9rem;
  font-weight: bold;
  align-items: center;
  align-content: center;
  text-align: center;
}
.highButton{
  background-color: #ff4124;
  color: #000000;
}
.contents {
  margin-top: 50px;
  width: 100%;
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  padding-left: 20px;
  padding-right: 20px;
  width: 90%;

}
.card h3 {
  font-size: 2rem;
  font-weight: bold;
  font-family: 'Instrument Serif', serif;
  color: #000000;
  text-align: center;
}

.price {
  color: #000000;
  font-size: 2.1rem;
  font-weight: bold;
  padding-bottom: 20px;
  padding-top: 20px;
  text-align: center;
}

ul {
  list-style: none;
  padding: 0;
  margin: 0 0 30px;
  width: 100%;
}

ul li {
  color: #000000;
  font-size: 1.1rem;
  margin-bottom: 12px;
  padding-left: 20px;
  position: relative;
  padding-top: 20px;
}

ul li::before {
  content: '✔';
  position: absolute;
  left: 0;
  color: #000000;
  font-weight: bold;
}

.btn,

 .btn {
  background-color: #000000;
  color: rgb(255, 255, 255);
  font-weight: bold;
  padding: 12px 20px;
  border: none;
  border-radius: 8px;
  text-align: center;
  width: 100%;
  align-self: baseline;
  cursor: pointer;
  font-size: 1.2rem;
  margin-top: auto;
}
.btn:hover{
    background-color: #ff4124;
    color: #ffffff;
}
.highButton{
  background-color: #ff4124;
  color: #000000;
}
.highButton:hover{
   background-color: #000000;
  color: #ff4124;
}
@media (max-width: 840px) {
  .card {
    position: relative;
    margin-top: 10px;
  }
  .pricing-cards {
    /* background-color: #4a0c0c; */
    margin-top: -0.04rem;
  }
  .card h3{
    font-size: 1.5rem;
  }

  .pricing-section h2 {
    font-size: 2rem;
  }
  .highlight {
    margin-top: 20px;
  }
}
</style>
