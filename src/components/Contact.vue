<template>
  <div class="contact" id="contact">
      <div class="container">
          <h1>Contact</h1>
          <div class="contact-form">
            <form 
            class="gform" 
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
                <input type="submit" value="Let's chat">
            </form>
          </div>
          <div class="thankyou-message">
            <!-- <h2><em>Thanks</em> for reaching out!</h2> -->
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
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

    .contact h6 {
        font-size: 2.5rem;
        text-align: center;
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
    }

    textarea {
        width: 100%;
    }

    input[type="submit"] {
        width: 30%;
        margin-left: 20rem;
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
}

.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>