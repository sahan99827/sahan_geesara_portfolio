<template>
  <div class="row">
      <div class="col-md-6">
        <div class="margH1">
          <h1><strong><em>Sahan Geesara</em></strong></h1>
          <h5 class="mb-4"><strong><em>FullStack Developer</em></strong></h5>
          <p>Hi! I'm creative Developer Based in Sri Lanka, and <br /> I'm Very passionate and dedicated to my work</p>
          <p><i class="bi bi-star-fill"></i> Quick Learner</p>
          <p><i class="bi bi-star-fill"></i> A Team Player</p>
          <p><i class="bi bi-star-fill"></i> Hard Worker</p>
          <div class="row marg">
            <a href="https://www.instagram.com/sahan_g_samarawicrama_?igsh=czNwaHV4ZmhqZ2s5" target="_blank"><i class="icon bi bi-instagram"></i></a>
            <a href="https://www.linkedin.com/in/sahan-g-samaravickrama-83b5001aa/" target="_blank"><i class="icon bi bi-linkedin"></i></a>
            <a href="https://github.com/sahan99827" target="_blank"><i class="icon bi bi-github"></i></a>
          </div>
        </div>

    </div>
    <div class="col-md-6 mt-5 mb-5">
      <div>
        <img src="/assets/1.png" alt="Image Description" style="width:300px; height:400px">
      </div>
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
.icon{
  margin-top: 10px !important;
  font-size: 40px !important;
}
a{
  text-decoration: none;
  color:black;
}
.marg{
  margin-top: -260px !important;
  margin-left: -140px !important;
}
.margH1{
  margin-top: 90px !important;
  margin-left: 140px !important;

}
@media (max-width: 490px) {
  img {
    width: auto  !important;
    height: auto  !important;
    margin-top: 30px !important;
    margin-left: 60px !important;
    align-content: center;
  }
  h1{
    margin-top: 60px !important;
    text-align: center;
  }
  h5{
    text-align: center;
  }
  .margH1{
    margin-top: -50px !important;
    margin-left: 140px !important;
    margin-bottom: 60px;
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