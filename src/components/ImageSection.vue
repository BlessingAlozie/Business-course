<template>
  <div class="image"></div>
</template>

<style scoped>
.image {
  width: 100%;
  height: 100vh;
  background-color: black;
  background-image: url('/women.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

/* Tablet */
@media (max-width: 1024px) {
  .image {
    height: 70vh; /* reduce height */
    background-position: top center; /* show top part better */
  }
}

/* Mobile */
@media (max-width: 768px) {
  .image {
    height: 50vh; /* shorter height for phones */
    background-size: cover; /* fit whole image */
    background-position: center;
  }
}
</style>
