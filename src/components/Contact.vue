<template>
  <div class="textCenter mt-5 mb-5">
    <h1 style="font-weight: bold"> Get in Touch</h1>
    <p>Contact Me</p>
  </div>
    <div class="row justify-content-center mt-5 mb-5">
      <div class="col-md-6">
        <div class="row justify-content-center">
          <div class="card col-md-4 m-3" style="width: 11.9rem;border-radius: 15px;">
            <div class="card-body">
              <div class="align-content-center">
                <i class="bi bi-envelope"></i>
              </div>
              <h4> Email </h4>
              <p>geesarasahan0123@gmail.com</p>
            </div>
          </div>
          <div class="card col-md-4 m-3" style="width: 11.5rem;border-radius: 15px;">
            <div class="card-body">
              <i class="bi bi-whatsapp"></i>
              <h4> Whatsapp </h4>
              <p>+94 78 8392 166</p>
            </div>
          </div>
          <div class="card col-md-4 m-3" style="width: 11rem;border-radius: 15px;">
            <div class="card-body">
              <i class="bi bi-facebook"></i>
              <h4> Facebook </h4>
              <p> sahan-g-samaravicrama</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <form ref="form" @submit.prevent="sendEmail">
          <div class="form-floating mb-3">
            <input type="text" class="form-control" id="floatingInput"   name="user_name" placeholder="Nuwan Sandeep">
            <label for="floatingInput" class="form-label">Name</label>
          </div>
          <div class="form-floating mb-3">
            <input type="email" class="form-control"
                   id="exampleFormControlInput2"  name="form_email" placeholder="name@example.com">
            <label for="exampleFormControlInput2" class="form-label">Email </label>
          </div>
          <div class="form-floating mb-5">
            <textarea class="form-control" id="exampleFormControlTextarea1" name="message"  rows="12"></textarea>
            <label for="exampleFormControlTextarea1" class="form-label" style="height: 200px">Message</label>
          </div>
          <button type="submit" class="btn btn-dark mb-5 mt-5" style="width: 300px;height: 60px;border-radius: 20px">Send Message <i class="bi bi-send"></i> </button>
        </form>
      </div>
    </div>
</template>
<script>
import emailjs from '@emailjs/browser';

export default {
  methods: {
    sendEmail() {
      emailjs
          .sendForm('service_jfkxjtz', 'template_1uxngrt', this.$refs.form, {
            publicKey: 'E3o89W-UvbW1YLFjg',
          })
          .then(
              () => {
                console.log('SUCCESS!');
              },
              (error) => {
                console.log('FAILED...', error.text);
              },
          );
    },
  },
};
</script>
<style scoped>
.textCenter{
  text-align: center;
}
.card{
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.3); /* Adds a shadow effect */

}
</style>