<template>
  <div class="container" id="syllabus">
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
        <!-- <img src="/cross.svg" alt="" /> More -->
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
    date: "THU (8/21), 5:00 PM WAT / 12:00 PM ET",
    topic: "Discovering Your VA Superpower: Skills Assessment",
  },
  {
    date: "MON (8/25), 5:00 PM WAT / 12:00 PM ET",
    topic: "Setting Up Your Home Office on a Budget",
  },
  {
    date: "THU (8/28), 5:00 PM WAT / 12:00 PM ET",
    topic: "Time Management and Work-from-Home Strategies for Moms",
  },
  {
    date: "MON (9/1), 5:00 PM WAT / 12:00 PM ET",
    topic: "Client Communication and Time Management",
  },
  {
    date: "THU (9/4), 5:00 PM WAT / 12:00 PM ET",
    topic: "Email Handling, Scheduling & Calendar Tools",
  },
  {
    date: "MON (9/8), 5:00 PM WAT / 12:00 PM ET",
    topic: "Social Media Content Creation & Management",
  },
  {
    date: "THU (9/11), 5:00 PM WAT / 12:00 PM ET",
    topic: "Basic Graphic Design Using Canva",
  },
  {
    date: "MON (9/15), 5:00 PM WAT / 12:00 PM ET",
    topic: "Creating Your First Client Proposal Template",
  },
  {
    date: "THU (9/18), 5:00 PM WAT / 12:00 PM ET",
    topic: "Pricing Your Services Like a Pro",
  },
  {
    date: "MON (9/22), 5:00 PM WAT / 12:00 PM ET",
    topic: "How to Get Clients (Even Without Experience)",
  },
  {
    date: "THU (9/25), 5:00 PM WAT / 12:00 PM ET",
    topic: "Using Freelance Platforms & Networking",
  },
  {
    date: "MON (9/29), 5:00 PM WAT / 12:00 PM ET",
    topic: "Building Your Online Presence & Portfolio",
  },
  {
    date: "THU (10/2), 5:00 PM WAT / 12:00 PM ET",
    topic: "Client Contracts, Invoicing & Getting Paid",
  },
  {
    date: "MON (10/6), 5:00 PM WAT / 12:00 PM ET",
    topic: "Professional VA Communication: Write Like a Pro",
  },
  {
    date: "THU (10/9), 5:00 PM WAT / 12:00 PM ET",
    topic: "Handling Feedback & Managing Difficult Clients",
  },
  {
    date: "MON (10/13), 5:00 PM WAT / 12:00 PM ET",
    topic: "Graduation Day: Pitch Yourself & Launch Your VA Journey!",
  },
];
</script>

<style scoped>
.container {
  width: 100%;
  padding: 0 100px;
  margin-top: 100px;
  color: #000000;
  font-family: Nekst, sans-serif;
}

.heading {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 50px;
  text-transform: uppercase;
}

.module {
  width: 100%;
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
}

.info {
  flex: 1;
  min-width: 250px;
}

.info h1 {
  font-size: 2rem;
  font-weight: 700;
  margin-top: 10px;
}

.info h3 {
  font-size: 1.2rem;
  font-weight: 600;
  color: #FF4124;
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
