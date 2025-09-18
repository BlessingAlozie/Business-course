<template>
  <div class="container-wrapper">
    <div class="container">
      <h2>
        Early bird pricing ends in <br />
        <span>04 hours.</span> <b>REGISTER NOW TO save ₦10,000</b>
      </h2>

      <h1>{{ format(hours) }} : {{ format(minutes) }} : {{ format(seconds) }}</h1>


      <button class="hvr-icon-forward">
        Join The Bootcamp &nbsp;&nbsp;&nbsp;&nbsp;
        <i class="fa-solid fa-arrow-right hvr-icon"></i>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hours: 4,
      minutes: 0,
      seconds: 0,
      timer: null,
    };
  },
  mounted() {
    this.startCountdown();
  },
  beforeUnmount() {
    clearInterval(this.timer); // cleanup
  },
  methods: {
    startCountdown() {
      this.timer = setInterval(() => {
        if (this.seconds > 0) {
          this.seconds--;
        } else {
          if (this.minutes > 0) {
            this.minutes--;
            this.seconds = 59;
          } else {
            if (this.hours > 0) {
              this.hours--;
              this.minutes = 59;
              this.seconds = 59;
            } else {
              clearInterval(this.timer); // stop at 0
            }
          }
        }
      }, 1000);
    },
    format(num) {
      return num < 10 ? "0" + num : num;
    },
  },
};
</script>

<style scoped>
.container-wrapper {
  width: 100%;
  font-family: 'Montserrat', sans-serif;
  background-color: #000000;
  text-align: center;
padding-top: 80px;
height: auto;

}

.container {
  color: #ffffff;
   margin: auto;
   padding-bottom: 80px;
   padding-left: 50px;
   padding-right: 50px;
}

.container h2 {
  font-size: 2.5rem;
  font-weight: 300;
  text-transform: uppercase;
  margin: auto;
  line-height: 3rem;
  max-width: 800px;

}

.container h1 {
  font-size: 8rem;
  font-weight: 700;
  margin-top: 40px;
  color: #FF4124;
}

.container span {
  color: #FF4124;
  font-size: 3rem;
  font-weight: 700;
}

.container b {
  font-size: 2.5rem;
  font-weight: 700;
}

button {
  margin-top: 40px;
  background-color: #232323;
  color: white;
  border: none;
  padding: 20px 60px;
  font-size: 20px;
  font-weight: 600;
  cursor: pointer;
  border-radius: 6px;
  transition: all 0.3s ease;
}

button:hover {
  background-color: #FF4124;
}

/* ✅ Tablet */
@media (max-width: 1024px) {
  .container h2 {
    font-size: 2rem;
    line-height: 2.8rem;
  }
  .container h1 {
    font-size: 6rem;
  }
  button {
    padding: 18px 50px;
    font-size: 18px;
  }
}

/* ✅ Mobile */
 @media (max-width: 625px) {


  .container h1 {
    font-size: 4rem;
  }

}

/* ✅ Small Mobile */
@media (max-width: 480px) {
  .container h2 {
    font-size: 1.4rem;
    line-height: 2rem;
  }
  .container h1 {
    font-size: 2.8rem;
  }
  .container span,
  .container b {
    font-size: 1.5rem;
  }
  button {
    padding: 14px 30px;
    font-size: 15px;
  }
}
</style>
