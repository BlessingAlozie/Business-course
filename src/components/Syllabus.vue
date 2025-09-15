<template>
  <div class="wrapper" >
    <h2 class="heading">Syllabus</h2>

    <div
      class="module"
      v-for="(item, index) in syllabus"
      :key="index"
    >
      <div class="number">{{ index < 10 ? '0' + index : index }}</div>
      <div class="info">
        <h3>{{ item.date }}</h3>
        <h1 class="title">{{ item.topic }}</h1>
        <p>{{ item.subtitle }}</p>
      </div>
      <div class="duration">
        <img src="/cross.svg" alt="" /> More

      </div>
    </div>
  </div>
</template>

<script setup>
const syllabus = [
  {
    date: "SAT (Start Date), 10:00 AM WAT / 5:00 AM ET",
    topic: "Orientation & Program Kickoff",
    subtitle: "Welcome, expectations, accountability system",
  },
  {
    date: "SAT (Week 1), 10:00 AM WAT / 5:00 AM ET",
    topic: "Foundation & Business Idea Validation",
    subtitle: "Validate ideas, feasibility analysis, entrepreneurial mindset",
  },
  {
    date: "SAT (Week 2), 10:00 AM WAT / 5:00 AM ET",
    topic: "Business Model & Planning",
    subtitle: "Revenue streams, pricing, financial roadmap, business plan framework",
  },
  {
    date: "SAT (Week 3), 10:00 AM WAT / 5:00 AM ET",
    topic: "Legal Structure & Registration",
    subtitle: "Choose structure, complete registration, ensure compliance",
  },
  {
    date: "SAT (Week 4), 10:00 AM WAT / 5:00 AM ET",
    topic: "Financial Management & Setup",
    subtitle: "Accounting systems, cash flow management, business credit",
  },
  {
    date: "SAT (Week 5), 10:00 AM WAT / 5:00 AM ET",
    topic: "Marketing Strategy & Brand Development",
    subtitle: "Brand identity, multi-channel marketing, digital presence",
  },
  {
    date: "SAT (Week 6), 10:00 AM WAT / 5:00 AM ET",
    topic: "Sales & Customer Acquisition",
    subtitle: "Sales skills, acquisition systems, retention & referrals",
  },
  {
    date: "SAT (Week 7), 10:00 AM WAT / 5:00 AM ET",
    topic: "Operations & Systems",
    subtitle: "Automation, scalability, team planning",
  },
  {
    date: "SAT (Week 8), 10:00 AM WAT / 5:00 AM ET",
    topic: "Launch Preparation & Growth Strategy",
    subtitle: "Launch plan, long-term growth, accountability system",
  },


];
</script>

<style scoped>

.wrapper{
  width: 100%;

}
.heading {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 50px;
  text-transform: uppercase;
  padding-left: 100px;
  font-family: 'Instrument Serif', serif;
}

.module {
  width: 90%;
  margin: auto;
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  margin-top: 40px;
  gap: 40px;
  flex-wrap: wrap;
  padding-bottom: 30px;
  border-bottom: 1px solid rgba(29, 28, 28, 0.2);

}

.number {
  font-size: 9rem;
  font-weight: 800;
  color: #000000;
  flex-shrink: 0;
  line-height: 1;
  width: 20%
}

.info {

  min-width: 250px;
  /* margin-left: 12px; */
 line-height: 1;
 /* background-color: #fff; */
 width: 60%;
}

.info h1 {
  font-size: 3rem;
  font-weight: 550;
   font-family: 'Instrument Serif', serif;
  /* margin-top: 10px; */
  line-height: 0.5;

}

.info h3 {
  font-size: 1.2rem;
  font-weight: 600;
  color: #FF4124;



}

.info p{
  font-size: 1.2rem;
  font-weight: 600;
  color: #868686;

}


.duration {
  font-size: 1.2rem;
  font-weight: 600;
  display: flex;
  align-items: center;
  white-space: nowrap;
  flex-shrink: 0;
}

.duration img {
  width: 20px;
  height: 20px;
  margin-right: 8px;
}

/* 📱 Tablet */
@media (max-width: 768px) {
  .container {
    padding: 0 20px;
    text-align: center;
  }

  .module {
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }

  .number {
    font-size: 4rem;
  }

  .info h1 {
    font-size: 1.4rem;
  }

  .info h3 {
    font-size: 1rem;
  }

  .duration {
    font-size: 1rem;
  }
}

/* 📱 Small Mobile */
@media (max-width: 480px) {
  .number {
    font-size: 3rem;
  }

  .info h1 {
    font-size: 1.1rem;
  }

  .info h3 {
    font-size: 0.9rem;
  }

  .duration {
    font-size: 0.9rem;
  }
}
</style>
