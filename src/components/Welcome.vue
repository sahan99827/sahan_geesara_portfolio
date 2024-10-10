<template>
  <div class="row">
    <div class="col-md-6">
      <img src="/assets/1.png" alt="Image Description" style="width:400px; height:500px"  >
    </div>
    <div class="col-md-6">
      <h1><strong><em>Sahan Geesara</em></strong></h1>
      <h5><strong><em>FullStack Developer</em></strong></h5>
      <p>Hi! I'm creative Developer Based in Sri Lanka, and <br /> I'm Very passionate and dedicated to my work</p>
      <p><i class="bi bi-star-fill"></i> Quick Learner</p>
      <p><i class="bi bi-star-fill"></i> A Team Player</p>
      <p><i class="bi bi-star-fill"></i> Hard Worker</p>
    </div>
  </div>

</template>

<style scoped>
@media (max-width: 768px) {
  img {
    width: 100%;
    height: auto;
  }
}

@media (max-width: 490px) {
  img {
    margin-top: 20px !important;
  }
  img:hover {
    transform: none;
  }
}

img {
  object-fit: cover;
  border-radius: 180px;
  border: #042eff 10px solid;
  box-shadow: 0 30px 50px rgb(255, 255, 255);
  transition: transform 5s ease, border 5s ease; /* Add transition for smooth animation */
  animation: border-animation 5s infinite;
}
h1:hover {
    color: #0128f6;
}
/* Keyframes for border animation */
@keyframes border-animation {
  0% {
    border-color: #3aff04;
    box-shadow: 0 30px 50px rgb(240, 241, 246);
  }
  50% {
    border-color: rgba(3, 1, 1, 0.7); /* Change to another color */
    box-shadow: 0 30px 50px rgb(225, 193, 193); /* Add glowing effect */
  }
  100% {
    border-color: #042eff;
    box-shadow: 0 30px 50px rgb(255, 255, 255);
  }
}
</style>
<script setup>
</script>