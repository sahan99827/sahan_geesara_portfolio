<template>
  <div class="textCenter mt-5 mb-5">
    <h1 style="font-weight: bold"> Certificates</h1>
    <p>What i archived</p>
  </div>
  <div class="row justify-content-center mt-5 mb-5">
      <div class="col-md-4 mb-5">
        <img class="image" src="/assets/Certificates/1.jpeg" alt="Image Description" width="400px">
      </div>
      <div class="col-md-4 mb-5">
          <img class="image" src="/assets/Certificates/2.jpeg" alt="Image Description" width="400px">
      </div>
      <div class="col-md-4 mb-5">
        <img class="image" src="/assets/Certificates/3.jpeg" alt="Image Description" width="400px">
      </div>
      <div class="col-md-4 mb-5">
        <img class="image" src="/assets/Certificates/4.jpeg" alt="Image Description" width="400px" height="290px">
      </div>
      <div class="col-md-4 mb-5">
        <img class="image" src="/assets/Certificates/5.jpeg" alt="Image Description" width="400px">
      </div>
  </div>
</template>
<style scoped>
.textCenter{
  text-align: center;
}
.image {
  transition: transform 0.4s ease, box-shadow 0.4s ease;
  box-shadow: 0px 35px 24px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */
  border: black 2px solid;
}

/* Animation on mouse hover */
.image:hover {

  transform: scale(1.5); /* Enlarges and rotates the image slightly */
  box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */
}
</style>
<script setup>
</script>