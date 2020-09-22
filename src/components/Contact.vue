<template>
  <div class="contact" id="contact">
      <div class="container">
          <h1>Contact</h1>
          <h6>Lets chat</h6>
          <form action="">
              <label for="name">Name:</label>
              <input type="text" id="name" name="name" placeholder="Enter your name" required>
              <label for="email">Email:</label>
              <input type="email" id="email" name="email" placeholder="Please enter your email" required>
              <label for="subject">Subject:</label>
              <textarea name="subject" id="subject" cols="10" rows="10"></textarea>
              <input type="submit" value="submit">
          </form>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>