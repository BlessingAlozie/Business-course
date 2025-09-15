<template>
  <div class="container">
  <section class="contact-section">
    <h2 class="form-heading">Get In Touch</h2>
    <p class="form-subheading">
      Please fill the form, we will be happy to assist you.
    </p>

    <form class="contact-form">
      <!-- Name + Email side by side -->
      <div class="form-row">
        <input type="text" placeholder="Name" class="form-input" />
        <input type="email" placeholder="Email" class="form-input" />
      </div>

      <!-- Message -->
      <textarea
        placeholder="Message"
        class="form-textarea"
        rows="8"
      ></textarea>

      <!-- Button -->
      <button type="submit" class="form-btn">Submit</button>
    </form>
  </section>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
};
</script>

<style scoped>
.container{
  width: 100vw;
  background-color: #ffffff;
  padding-top: 80px;
  padding-bottom: 80px;

}
.contact-section {
  max-width: 700px;
  margin: 0 auto;
  text-align: center;
  padding: 0  2rem 2rem 2rem  ;
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.1);
  font-family: 'Montserrat', sans-serif;
}

.form-heading {
  font-size: 4rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
  font-family: 'Montserrat', sans-serif;
}

.form-subheading {
  font-size: 1.5rem;
  color: #333;
  margin-bottom: 2rem;
}
/* Form styling */
.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 100%;

}

.form-row {
  display: flex;
  gap: 1rem;
}

.form-input,
.form-textarea {
  flex: 1;
  padding: 15px;
  border: 1px solid #ccc;
  border-radius: 8px;
  font-size: 1rem;
  font-family: "Montserrat", sans-serif;
}

.form-textarea {
  resize: vertical;
}

.form-btn {
  background-color: #000;
  color: #fff;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  padding: 20px;
  border-radius: 8px;
  cursor: pointer;
  transition: 0.3s ease;
}

.form-btn:hover {
  background-color: #ff4124;
}

/* Responsive */
@media (max-width: 768px) {
  .form-row {
    flex-direction: column;
  }
}

</style>
