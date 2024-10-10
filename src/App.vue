<script setup>
import {RouterView } from 'vue-router'
</script>

<template>
  <div>
    <nav class="navbar navbar-expand-lg bg-light bg-body fixed-top">
      <div class="container">
        <a class="navbar-brand" href="#home">Sahan</a>
        <button class="navbar-toggler" type="button"
                data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-center" id="navbarSupportedContent">

          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#home">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#about">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#project">Project</a>

            </li>
            <li class="nav-item">
              <a class="nav-link" href="#skills">Skills</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#education">Education</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#certificate">Certificates</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#experience">Work experience</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>
        </div>

      </div>
    </nav>
  </div>
  <div>
    <RouterView />
  </div>
</template>

<style>
nav {
  display: inline-block;
  position: fixed;
  margin-left: 0;
  font-family: Arial,serif;
  right: 0;
}

</style>
