<template>
  <div v-if="showModal" class="modal-overlay" @click.self="$emit('close')">
    <div class="modal">
      <i class="fa-solid fa-xmark close-icon" @click="$emit('close')"></i>


       <!-- Left side (image with overlay text) -->
   <div class="modal-image">
    <div class="overlay-text">
      <h2>Join Our Program</h2>
      <p>Transform your skills and achieve your business goals with expert guidance.</p>
    </div>
  </div>


      <!-- Right side (form) -->
      <div class="modal-form">

        <h2>Create Your Account</h2>
        <p class="subtitle">Enroll now and start learning today</p>

        <form @submit.prevent="submitForm">
          <div class="form-grid">
            <!-- First & Last Name -->
            <div>
              <label for="firstName">First Name</label>
              <input
                id="firstName"
                type="text"
                v-model="form.firstName"
                placeholder="Enter first name"
                required
              />
            </div>
            <div>
              <label for="lastName">Last Name</label>
              <input
                id="lastName"
                type="text"
                v-model="form.lastName"
                placeholder="Enter last name"
                required
              />
            </div>

            <!-- Email -->
            <div class="full-width">
              <label for="email">Email Address</label>
              <input
                id="email"
                type="email"
                v-model="form.email"
                placeholder="Enter your email"
                required
              />
            </div>

            <!-- Phone -->
            <div>
              <label for="phone">Phone Number</label>
              <input
                id="phone"
                type="tel"
                v-model="form.phone"
                placeholder="+234 800 000 0000"
                required
              />
            </div>

            <!-- Country -->
            <div>
              <label for="country">Country</label>
              <select id="country" v-model="form.country" required>
                <option value="" disabled>Select your country</option>
                <option v-for="country in countries" :key="country" :value="country.toLowerCase()">
                  {{ country }}
                </option>
              </select>
            </div>
          </div>

          <button type="submit" class="form-btn">Enroll Now</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['showModal'],
  data() {
    return {
      form: {
        firstName: '',
        lastName: '',
        email: '',
        phone: '',
        country: '',
        password: '',
      },
      countries: [
        'Nigeria',
        'Ghana',
        'Kenya',
        'South Africa',
        'Uganda',
        'Tanzania',
        'Rwanda',
        'Ethiopia',
        'Cameroon',
        'Ivory Coast',
        'Senegal',
        'Mali',
        'Burkina Faso',
        'Niger',
        'Guinea',
        'Benin',
        'Togo',
        'Sierra Leone',
        'Liberia',
        'Gambia',
        'Mauritania',
        'Chad',
        'Central African Republic',
        'Republic of the Congo',
        'Democratic Republic of the Congo',
        'Gabon',
        'Equatorial Guinea',
        'Sao Tome and Principe',
        'Cape Verde',
        'Guinea-Bissau',
        'Comoros',
        'Seychelles',
        'Mauritius',
        'Madagascar',
        'Mozambique',
        'Zimbabwe',
        'Botswana',
        'Namibia',
        'Zambia',
        'Malawi',
        'Lesotho',
        'Eswatini',
        'Angola',
        'Burundi',
        'Djibouti',
        'Eritrea',
        'Somalia',
        'Sudan',
        'South Sudan',
        'Libya',
        'Tunisia',
        'Algeria',
        'Morocco',
        'Egypt',
      ],
    }
  },
  methods: {
    submitForm() {
      console.log('Form submitted:', this.form)
      this.$emit('close')
    },
  },
}
</script>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
}

.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.6);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 10000;
  backdrop-filter: blur(3px);
}

.modal {
  display: flex;
  background: #fff;
  border-radius: 16px;
  overflow: hidden;
  width: 900px;
  max-width: 95%;
  box-shadow: 0 20px 50px rgba(0, 0, 0, 0.25);
  animation: fadeIn 0.3s ease;
  position: relative;
}

.close-icon {
  position: absolute;
  top: 20px;
  right: 20px;
  font-size: 1.8rem;
  color: #000000;
  cursor: pointer;
  z-index: 10001;
  transition: color 0.2s ease;
}

.close-icon:hover {
  color: #ff4124;
}


/* Left image side */
.modal-image {
  flex: 1;
  background: url('/signup-image.svg') center/cover no-repeat;
  object-fit: cover;
  position: relative;
  min-height: 300px; /* ensures visibility on smaller screens */

}
.overlay-text {
  position: absolute;
  bottom: 20px;
  left: 20px;
  color: white;
  background: rgba(0, 0, 0, 0.55);
  padding: 1rem 1.5rem;
  border-radius: 8px;
  max-width: 80%;
}
.overlay-text h2 {
  margin: 0;
  font-size: 1.5rem;
}
.overlay-text p {
  font-size: 0.9rem;
  margin-top: 0.3rem;
  line-height: 1.3;
}

/* Right form side */
.modal-form {
  flex: 1;
  padding: 2.5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.modal-form h2 {
  margin-bottom: 0.5rem;
  font-size: 1.8rem;
  font-weight: 700;
  color: #222;
}
.subtitle {
  color: #666;
  margin-bottom: 2rem;
  font-size: 0.95rem;
}

.modal-form form {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  max-width: 100%;
}

/* Grid layout */
.form-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1.5rem; /* reduced from 2.5rem */
}
.full-width {
  grid-column: span 2;
}

.modal-form label {
  font-size: 0.85rem;
  font-weight: 500;
  color: #444;
  margin-bottom: 0.35rem;
  display: block;
}
.modal-form input,
.modal-form select {
  width: 100%;
  padding: 12px 14px;
  border: 1px solid #ccc;
  border-radius: 8px;
  font-size: 0.95rem;
  outline: none;
  transition:
    border 0.2s,
    box-shadow 0.2s;
}
.modal-form input:focus,
.modal-form select:focus {
  border-color: #ff4124;
  box-shadow: 0 0 0 2px rgba(255, 65, 36, 0.2);
}

.form-btn {
  margin-top: 1rem;
  background: #ff4124;
  color: #fff;
  border: none;
  padding: 14px;
  border-radius: 10px;
  cursor: pointer;
  font-size: 1rem;
  font-weight: 600;
  transition:
    background 0.3s ease,
    transform 0.2s ease;
}
.form-btn:hover {
  background: #e2361b;
  transform: translateY(-2px);
}

/* Animation */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(15px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* --------------------- */
@media (max-width: 768px) {
  .modal {
    flex-direction: column; /* stack vertically */
    width: 95%;
    height: auto;
     border-radius: 16px;
     margin-top: 80px;

  }

  .modal-image {
    width: 100%; /* full width */
    height: 500px; /* fixed height */
    flex: none;
    background-size: cover;
    background-position: top ;
    display: none;


  }

  .modal-form {
    width: 100%; /* full width */
    padding: 1.5rem;
  }

  .form-grid {
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  .full-width {
    grid-column: span 1;
  }

  .form-btn {
    width: 100%; /* button stretches full width */
    padding: 12px;
    box-sizing: border-box;
  }
  .modal-overlay {
  overflow-y: auto;
  padding: 2rem 1rem;
}

}

@media (max-width: 480px) {
  .modal-image {
    height: 150px; /* smaller height for very small screens */
  }

  .modal-form {
    padding: 1rem;
  }
  /* .modal-overlay {
  overflow-y: auto;
  padding: 2rem 1rem;
} */

}


</style>
