<template>
  <div class="textCenter mt-5 mb-5">
    <h1 style="font-weight: bold"> Certificates</h1>
    <p>What i Achieved</p>
  </div>
  <div class="row justify-content-center mt-5 mb-5" id="cetificateContainer">
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
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/6.jpg" alt="Image Description" width="400px">
    </div>
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/7.png" alt="Image Description" width="400px">
    </div>
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/8.png" alt="Image Description" width="400px" height="275px">
    </div>
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/9.png" alt="Image Description" width="400px" height="275px">
    </div>
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/10.png" alt="Image Description" width="400px" height="275px">
    </div>
    <div class="col-md-4 mb-5">
      <img class="image" src="/assets/Certificates/11.png" alt="Image Description" width="400px" height="275px">
    </div>
  </div>
  <div class="text-center m-4">
    <button id="prev" class="btn btn-dark m-2">Previous</button>
    <button id="next" class="btn btn-dark m-2">Next</button>
  </div>
</template>
<style scoped>
.textCenter {
  text-align: center;
}

.image {
  transition: transform 0.4s ease, box-shadow 0.4s ease;
  box-shadow: 0px 35px 24px rgba(0, 0, 0, 0.3);
  /* Adds a shadow effect */
  border: black 2px solid;
}

/* Animation on mouse hover */
.image:hover {

  transform: scale(1.5);
  /* Enlarges and rotates the image slightly */
  box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.3);
  /* Adds a shadow effect */
}

@media (max-width: 490px) {
  .image {
    width: 300px !important;
    height: 180px;
    margin-left: 45px !important;
    box-shadow: 0px 65px 44px rgba(0, 0, 0, 0.3);
    /* Adds a shadow effect */

  }

  .image:hover {
    transform: none;
    /* Enlarges and rotates the image slightly */
    box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.3);
    /* Adds a shadow effect */
  }
}

</style>
<script scoped>
document.addEventListener("DOMContentLoaded", () => {

  // Select all certificate items
  const cards = Array.from(document.querySelectorAll("#cetificateContainer .col-md-4"));
  const itemsPerPage = 3;
  let currentPage = 1;

  function renderPage() {
    const start = (currentPage - 1) * itemsPerPage;
    const end = start + itemsPerPage;

    cards.forEach((card, index) => {
      card.style.display = index >= start && index < end ? "block" : "none";
    });
  }

  document.getElementById("next").addEventListener("click", () => {
    if (currentPage * itemsPerPage < cards.length) {
      currentPage++;
      renderPage();
    }
  });

  document.getElementById("prev").addEventListener("click", () => {
    if (currentPage > 1) {
      currentPage--;
      renderPage();
    }
  });

  renderPage();
});
</script>
