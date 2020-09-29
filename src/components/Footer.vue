<template>
  <div class="copyright">
    <footer>
        <p>&copy; 2020 Adrian Avila</p>
        <div @click="scrollUp" ref="#" class="up" id="up">
            <i class="fa fa-chevron-up"></i>
        </div>
    </footer>
  </div>
</template>

<script>
export default {
  methods: {
    scrollUp () {
        document.getElementById('app').scrollIntoView({behavior: 'smooth'});
          let to = this.moveToDown
            ? this.$refs.description.offsetTop - 60
            : 0

            window.scroll({
              top: to,
              left: 0,
              behavior: 'smooth'
            })

            this.moveToDown = !this.moveToDown
    }
  }
}
</script>

<style scoped>

/* For mobile phones: */
@media only screen and (max-width: 600px) {
    [class*="col-"] {
    width: 100%;
    }


    .copyright {
      width: 100%;
      text-align: center;
      background: black;
      padding: 2rem;
      position: relative;
    }

    .up {
      position: absolute;
      width: 5rem;
      height: 5rem;
      background-color: lightgrey;
      top: -2.5rem;
      right: 2rem;
      border-radius: 100%;
      display: flex;
    }

    .up i {
      color: black;
      font-size: 2rem;
      margin: auto;
    }

    p {
      font-size: 1.3rem;
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