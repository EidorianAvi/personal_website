<template>
  <div class="copyright">
    <footer>
        <div class="up" id="up">
            <p>&copy; 2020 Adrian Avila</p>
        </div>
    </footer>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

/* For mobile phones: */
@media only screen and (max-width: 600px) {
    [class*="col-"] {
    width: 100%;
    }


    .copyright {
      max-width: 95%;
      display: flex;
      justify-content: flex-end;
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