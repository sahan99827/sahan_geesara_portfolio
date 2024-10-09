<template>

    <div class="textCenter">
      <h1 style="font-weight: bold"> Skills</h1>
      <p>My Technical Level</p>
    </div>

  <div class="container ">
    <div class="row justify-content-center">
      <div class="card col-md-4 m-3" style="width: 20rem;border-radius: 15px;">
        <div class="card-body">
          <h4 style="text-align: center;font-weight: bold !important;">FrontEnd</h4>
          <ul type="none">
            <li>Angular</li>
            <li>vue</li>
            <li>Html/CSS</li>
            <li>JavaScript</li>
          </ul>
        </div>
      </div>
      <div class="card col-md-4 m-3" style="width: 20rem;border-radius: 15px;">
        <div class="card-body">
          <h4 style="text-align: center;  font-weight: bold !important;">BackEnd</h4>
          <ul type="none">
            <li>PHP</li>
            <li>JAVA</li>
            <li>MySQL</li>
            <li>Laravel</li>
          </ul>
        </div>
      </div>
      <div class="card col-md-4 m-3" style="width: 20rem;border-radius: 15px;">
        <div class="card-body">
          <h4 style="text-align: center;  font-weight: bold !important;">Tool</h4>
          <ul type="none">
            <li>GitHub</li>
            <li>Jira</li>
            <li>Postman</li>
            <li>Intelli J</li>
            <li>PhpStorm</li>
          </ul>
        </div>
      </div>

    </div>
  </div>
</template>
<style scoped>
 .textCenter{
   text-align: center;
 }
 p{
   font-size: 18px;
 }
 li{
   font-size: 20px;
 }
 .card{
   box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */
 }
</style>
<script setup>
</script>