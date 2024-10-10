<template>
  <div class="row">
    <div class="col-md-6">
      <img src="/assets/1.png" alt="Image Description" style="width:400px; height:500px"  >
    </div>
    <div class="col-md-6">
      <h1><strong><em>Sahan Geesara</em></strong></h1>
      <h5 class="mb-4"><strong><em>FullStack Developer</em></strong></h5>
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
    width: auto;
    height: auto;
  }
}

@media (max-width: 490px) {
  img {
    width: auto;
    height: auto;
    margin-top: 20px !important;
    margin-right: 9px !important;
  }
  h1{
    margin-top: 60px !important;
    text-align: center;
  }
  h5{
    text-align: center;

  }
}

img {
  object-fit: cover;
  border-radius: 180px;
  border: rgba(238, 18, 18, 0.9) 5px solid;
  box-shadow: 0 30px 50px rgba(3, 1, 1, 0.7);
}
h1:hover {
    color: #0128f6;
}
</style>
<script setup>
</script>