<template>
  <div class="textCenter mt-5 mb-5">
    <h1 style="font-weight: bold"> About Me</h1>
    <p>My Introduction</p>
  </div>

  <div class="container">
    <div class="row justify-content-center mt-5 mb-5">
      <div class="col-md-6">
        <div class="row">
          <div class="card col-md-4 m-3" style="width: 11.9rem;border-radius: 15px;">
            <div class="card-body">
              <h4> Experience </h4>
              <span>6 Months Working</span>
            </div>
          </div>
          <div class="card col-md-4 m-3" style="width: 11.5rem;border-radius: 15px;">
            <div class="card-body">
              <h4> Completed </h4>
              <span>2+ Projects</span>
            </div>
          </div>
          <div class="card col-md-4 m-3" style="width: 11.1rem;border-radius: 15px;">
            <div class="card-body">
              <h4> Support </h4>
              <span>Online 24/7</span>
            </div>
          </div>
          <div class="col-md-4">
            <p><i class="bi bi-person-workspace"></i> Passionate Fullstack Developer with a knack for crafting innovative web solutions.</p>
          </div>
          <div class="col-md-4">
              <p><i class="bi bi-globe"></i> Fluent in both front-end and back-end technologies, I bring a holistic approach to web development.</p>
          </div>
          <div class="col-md-4">
            <p><i class="bi bi-pencil-fill"></i> Dedicated to staying updated with the latest trends and best practices in the tech world.</p>
          </div>
        </div>
        <button @click="downloadFile" class="btn btn-dark" style="width: 300px;height: 60px;border-radius: 20px"> Download Resume <i class="bi bi-file-earmark-pdf"></i> </button>
      </div>
      <div class="col-md-6">
        <img src="/assets/1.jpg" alt="Image Description" width="400px" height="300px" >
      </div>
    </div>
  </div>
</template>
<style scoped>
.textCenter{
  text-align: center;
}
@media (max-width: 768px) {
  img {
    width: 100%;
    height: auto;
  }
}
img{
  object-fit: cover;
  border-radius: 180px;

}
.card{
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */

}
</style>
<script setup>
const url = '/assets/Sahan_Geesara_CV.pdf'; // Replace with the actual path
function downloadFile() {
  const link = document.createElement('a');
  link.href = url;
  link.download = 'Sahan_Geesara_CV.pdf'; // Set the desired filename
  link.click();

  // If the file is generated dynamically (using a server-side API):
  // Make an API request to fetch the file data
  fetch('/api/download/file')
      .then(response => response.blob())
      .then(blob => {
        const url = URL.createObjectURL(blob);
        const link = document.createElement('a');
        link.href = url;
        link.download
            = 'Sahan_Geesara_CV.pdf';
        link.click();
        URL.revokeObjectURL(url);
      });
}
</script>