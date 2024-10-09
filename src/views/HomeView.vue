<script setup>
import Project from "@/components/Project.vue";
import Skills from "@/components/Skills.vue";
import Education from "@/components/Education.vue";
import WorkExperience from "@/components/WorkExperience.vue";
import Contact from "@/components/Contact.vue";
import About from "@/components/About.vue";
import Welcome from "@/components/Welcome.vue";
</script>

<template>
  <div class="home container">
    <div id="home"><Welcome /> </div>
    <div id="about"><About /> </div>
    <div class="container col-12" id="skills"><Skills /> </div>
    <div id="project"><Project /> </div>
    <div id="education"><Education /> </div>
    <div id="experience"><WorkExperience /> </div>
    <div id="contact"><Contact /> </div>

  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  .home {
    margin-top: 60px;
    height: 100vh;
    align-items: center;
  }
}
</style>