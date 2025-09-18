<template>
  <div class="wrapper">
    <h2 class="heading">Syllabus</h2>

    <div class="module" v-for="(item, index) in syllabus" :key="index">
      <div class="number">{{ index + 1 < 10 ? '0' + (index + 1) : index + 1 }}</div>
      <div class="info">
        <h3>{{ item.date }}</h3>
        <h1 class="title">{{ item.topic }}</h1>
        <p>{{ item.subtitle }}</p>
      </div>
      <div class="duration"><img src="/cross.svg" alt="" /> More</div>
    </div>
  </div>
</template>

<script setup>
const syllabus = [
  {
    date: 'SAT (Start Date), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Orientation & Program Kickoff',
    subtitle: 'Welcome, expectations, accountability system',
  },
  {
    date: 'SAT (Week 1), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Foundation & Business Idea Validation',
    subtitle: 'Validate ideas, feasibility analysis, entrepreneurial mindset',
  },
  {
    date: 'SAT (Week 2), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Business Model & Planning',
    subtitle: 'Revenue streams, pricing, financial roadmap, business plan framework',
  },
  {
    date: 'SAT (Week 3), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Legal Structure & Registration',
    subtitle: 'Choose structure, complete registration, ensure compliance',
  },
  {
    date: 'SAT (Week 4), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Financial Management & Setup',
    subtitle: 'Accounting systems, cash flow management, business credit',
  },
  {
    date: 'SAT (Week 5), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Marketing Strategy & Brand Development',
    subtitle: 'Brand identity, multi-channel marketing, digital presence',
  },
  {
    date: 'SAT (Week 6), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Sales & Customer Acquisition',
    subtitle: 'Sales skills, acquisition systems, retention & referrals',
  },
  {
    date: 'SAT (Week 7), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Operations & Systems',
    subtitle: 'Automation, scalability, team planning',
  },
  {
    date: 'SAT (Week 8), 10:00 AM WAT / 5:00 AM ET',
    topic: 'Launch Preparation & Growth Strategy',
    subtitle: 'Launch plan, long-term growth, accountability system',
  },
]
</script>

<style scoped>
.wrapper {
  width: 100%;
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 20px;
}

.heading {
  font-size: clamp(1.5rem, 4vw, 2.5rem);
  font-weight: 700;
  margin-bottom: 50px;
  text-transform: uppercase;
  font-family: 'Instrument Serif', serif;
  text-align: left;
}

.module {
  width: 100%;
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  margin-top: 40px;
  gap: clamp(20px, 4vw, 40px);
  padding-bottom: 30px;
  border-bottom: 1px solid rgba(29, 28, 28, 0.2);
}

.number {
  font-size: clamp(3rem, 8vw, 9rem);
  font-weight: 800;
  color: #000000;
  flex-shrink: 0;
  line-height: 1;
  width: clamp(80px, 15%, 150px);
  text-align: center;
}

.info {
  flex: 0 0 50%;
  min-width: 0; /* Allows text to shrink and wrap */
  line-height: 1.2;
  margin-left: 50px;
  /* background-color: #046a77; */
}

.info h1 {
  font-size: clamp(1.2rem, 4vw, 3rem);
  font-weight: 550;
  font-family: 'Instrument Serif', serif;
  margin: 8px 0;
  line-height: 1.1;
  word-wrap: break-word;
}

.info h3 {
  font-size: clamp(0.9rem, 2.5vw, 1.2rem);
  font-weight: 600;
  color: #ff4124;
  margin: 0 0 5px 0;
  word-wrap: break-word;
}

.info p {
  font-size: clamp(0.9rem, 2.5vw, 1.2rem);
  font-weight: 600;
  color: #868686;
  margin: 5px 0 0 0;
  word-wrap: break-word;
}

.duration {
  font-size: clamp(0.9rem, 2.5vw, 1.2rem);
  font-weight: 600;
  display: flex;
  align-items: center;
  flex-shrink: 0;
  margin-left: auto;
  min-width: fit-content;
}

.duration img {
  width: clamp(16px, 3vw, 20px);
  height: clamp(16px, 3vw, 20px);
  margin-right: 8px;
}

/* Desktop and Large Tablets */
@media (min-width: 1024px) {
  .wrapper {
    padding: 0 40px;
  }

  .heading {
    text-align: left;
    /* padding-left: 60px; */
  }

  .module {
    gap: 40px;
  }

  .number {
    width: 150px;
  }
}

/* Medium Tablets */
@media (max-width: 1023px) and (min-width: 769px) {
  .heading {
    margin-bottom: 40px;
  }

  .module {
    gap: 30px;
    flex-wrap: nowrap;
  }

  .number {
    width: 120px;
  }

  .duration {
    margin-left: 0;
    width: auto;
    margin-right: 100px;
  }
}

/* Small Tablets and Large Phones */
/* 📱 Tablet */
@media (max-width: 768px) {
  .module {
    flex-direction: row; /* ✅ keep row, no stacking */
    align-items: flex-start;
    gap: 15px;
    /* background-color: #1d1c6f;           */
  }

  .number {
    font-size: 4rem;
    width: auto;
    min-width: 60px;
  }
  .info {
    flex: 0 0 50%;

    margin: auto;
  }

  .info h1 {
    font-size: 1.4rem;
  }

  .info h3 {
    font-size: 0.95rem;
  }

  .info p {
    font-size: 0.9rem;
  }

  .duration {
    font-size: 0.95rem;

    margin-right: 50px;
  }
}

/* Small Mobile Phones */
@media (max-width: 480px) {
  .module {
    flex-direction: column; /* stack items vertically */
    align-items: flex-start; /* align to left */
    gap: 15px; /* spacing between number, info, duration */
  }

  .number {
    font-size: 2.5rem;
    width: 100%;
    text-align: left; /* align number left */
  }

  .info {
    width: 100%; /* take full width */
  }

  .info h1 {
    font-size: 1.2rem;
  }

  .info h3 {
    font-size: 0.9rem;
  }

  .info p {
    font-size: 0.85rem;
  }

  .duration {
    width: 100%;        /* full width below info */
    text-align: left;   /* align left */
    font-size: 0.9rem;
    margin-left: 0;     /* reset margin-left: auto */
    flex-shrink: 0;     /* keep it stable */
  }
}

</style>
