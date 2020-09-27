<template>
    <div class="row banner-page">
        <div class="col-12 banner-text">
            <h1>Adrian Avila</h1>
            <h6>Full Stack Software Engineer</h6>
        </div>
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

    .banner-text h6 {
        font-size: 1.75rem;
    }

    .banner-page {
        background: url('../assets/images/journey2.jpg') no-repeat center center fixed;
        background-size: 100% auto;
        display: flex;
        align-items: flex-start;
        height: 100vh;
    }


    .banner-text {
        margin-top: 30rem;
        font-family: 'Permanent Marker', cursive;
        text-align: center;
    }

    h1 {
        width: 100%;
        font-size: 6rem;
        background: rgb(232,232,236);
        /* background: linear-gradient(0deg, rgba(232,232,236,1) 0%, rgba(30,30,32,1) 100%); */
        background: linear-gradient(bottom-left #93a5cf  0%,  #e4efe9  100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    h6 { 
        font-size: 2rem;
        font-weight: 300;
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