<template>
  <div class="col-12 contact" id="contact"
        data-aos="fade-right"
        data-aos-delay="300"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
    >
      <div class="container">
          <h1>Contact</h1>
          <div class="contact-form">
            <form 
            class="gform pure-form pure-form-stacked" 
            method="POST" 
            action="https://script.google.com/macros/s/AKfycbwgxAEzOt1Zxd57Np597YokCibEbr4a8v8m8NfXZA/exec"
            data-email="reneavila1993@gmail.com" >
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Name" required>
                <label for="subject">Subject:</label>
                <input type="text" id="subject" name="subject" placeholder="Why you're reaching out" required><br>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Please enter your email" required><br>
                <label for="message">Message:</label>
                <textarea name="message" id="message" cols="10" rows="10" required></textarea><br>
                <input @click="sendMessage" type="submit" value="Let's chat">
            </form>
          </div>
          <div style="visibility:hidden;" id="thankyou_message">
            <h2><em>Thanks</em> for reaching out!</h2>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  methods: {
    sendMessage() {
      let form = document.querySelector('.gform');
      let thanksMessage = document.querySelector('#thankyou_message');
      
      setTimeout(() => {form.reset()}, 2500);
      setTimeout(() => {thanksMessage.style.visibility="visible"}, 2500);
      setTimeout(() => {thanksMessage.style.visibility="hidden"}, 5000);
    }
  }
}
</script>

<style scoped>
@media only screen and (max-width: 600px) {
    
    [class*="col-"] {
    width: 100%;
    }

    .contact { 
        display: flex;
        justify-content: center;
        align-items: center;
        max-width: 100%;
        height: 80vh;
    }

    .contact h1 { 
        font-size: 6rem;
        opacity: .5;
        text-align: center;
        margin-bottom: 2rem;
    }

    form {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    label {
        margin-top: 1rem;
        width: 100%;
        text-align: left;
        font-size: 1rem;
    }

    input {
        width: 100%;
        padding: .2rem 1rem;
    }

    textarea {
        width: 100%;
        padding: .5rem;
    }

    input[type="submit"] {
        width: 30%;
        margin-left: 18rem;
        margin-bottom: 2rem;
    }

    h2 {
      text-align: center;
    }

}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}

    .contact { 
        display: flex;
        justify-content: center;
        align-items: center;
        height: 80vh;
    }

    .container {
      width: 45vw;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content:center
    }

    .contact h1 { 
        font-size: 20rem;
        opacity: .5;
        text-align: center;
        margin-bottom: 2vh;
    }

    form {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    label {
        margin-top: 2vh;
        width: 100%;
        text-align: left;
        font-size: 6rem;
    }

    input {
        width: 100%;
        height: 2vh;
        font-size: 6rem;
        padding-left: 3rem;
    }

    textarea {
        width: 100%;
        height: 20vh;
        font-size: 6rem;
        padding: 1.5rem;
    }

    input[type="submit"] {
        font-size: 6rem;
        font-weight: bold;
        width: 15%;
        height: 3vh;
        margin-top: 2vh;
        margin-left: 35vw;
        margin-bottom: 4vh;
    }

    h2 {
      font-size: 10rem;
      text-align: center;
    }

}

.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>