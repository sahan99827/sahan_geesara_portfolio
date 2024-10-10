<template>
  <div class="textCenter m-5">
  <h1 style="font-weight: bold"> Education</h1>
  </div>
  <div class="row justify-content-center ">
    <div class="card col-md-12 m-3" style="width: 38rem;border-radius: 15px;">
      <div class="card-body m-4">
        <h4 style="text-align: center;font-weight: bold !important;">GCE Advanced Level Exam - 2018</h4>
        <p>Royal Central College - Polonnaruwa (2005 - 2018)</p>
        <p>Sat for the exam in commerce stream with ICT stream.</p>
      </div>
    </div>
  </div>
    <div class="row justify-content-center">
    <div class="card col-md-12 m-3" style="width: 38rem;border-radius: 15px;">
      <div class="card-body m-4">
        <h4 style="text-align: center;font-weight: bold !important;">GCE Ordinary Level Exam - 2015</h4>
        <p>Royal Central College - Polonnaruwa (2005 - 2018) </p>
        <p>Score 1A's 2B's 3C's 3Ss </p>
      </div>
    </div>
  </div>

</template>
<script setup>
</script>
<style scoped>
.textCenter{
  text-align: center;
}
.card{
  box-shadow: 0px 30px 20px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */
  border: black 2px solid;

}
@media (max-width: 490px) {
  .card {
    width:100% !important;
  }
}
p{
  text-align: center;
}
</style>