<template>
    <div class="row banner-page col-12" >
        <div class="col-12 banner-text">
            <h1>Adrian Avila</h1>
            <h6>Full Stack Software Engineer</h6>
            <div class="css-typing">
              <p>Star Wars Historian 🌌</p>
              <p>Shiba Dad 🐕</p>
              <p>Ramen Connoisseur 🍜</p>
            </div>
        </div>
    </div>
</template>

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
        width: 80vw;
        margin-left: 10vw; 
        margin-top: 22vh;
        font-family: 'Permanent Marker', cursive;
        text-align: center;
    }

    h1 {
        font-size: 5rem;
        background: rgb(232,232,236);
        /* background: linear-gradient(0deg, rgba(232,232,236,1) 0%, rgba(30,30,32,1) 100%); */
        background: linear-gradient(0deg, #93a5cf  0%,  #e4efe9  100%);
        -webkit-text-fill-color: transparent;
        -webkit-background-clip: text;
    }

    h6 { 
        font-size: 2rem;
        font-weight: 300;
    }

    .css-typing {
      margin-top: 2vh;
      margin-left: 22vw;
    }

    .css-typing p {
      border-right: .15em solid lightgray;
      font-size: 1.3rem;
      white-space: nowrap;
      overflow: hidden;
    }

    .css-typing p:nth-child(1) {
      width: 13em;
      -webkit-animation: type 2s steps(40, end);
      animation: type 2s steps(40, end);
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
    }

    .css-typing p:nth-child(2) {
      width: 11.5em;
      opacity: 0;
      -webkit-animation: type2 2s steps(40, end);
      animation: type2 2s steps(40, end);
      -webkit-animation-delay: 2s;
      animation-delay: 2s;
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
    }

    .css-typing p:nth-child(3) {
      width: 13em;
      opacity:  0;
      -webkit-animation: type3 5s steps(20, end), blink .5s step-end infinite alternate;
      animation: type3 5s steps(20, end), blink .5s step-end infinite alternate;
      -webkit-animation-delay: 4s;
      animation-delay: 4s;
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
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



    .banner-page {
      background: url('../assets/images/journey.jpg') no-repeat center fixed;
      background-size: 100% auto;
      display: flex;
      align-items: flex-start;
      height: 100vh;
    }

    .banner-text {
      width: 80vw;
      margin-left: 10vw; 
      margin-top: 22vh;
      font-family: 'Permanent Marker', sans-serif;
      text-align: center;
    }

    h1 {
      font-size: 33rem;
      background: rgb(232,232,236);
      background: linear-gradient(0deg, #93a5cf  0%,  #e4efe9  100%);
      -webkit-text-fill-color: transparent;
      -webkit-background-clip: text;
    }

    
    h6 { 
      font-size: 10rem;
      font-weight: 300;
    }

    .css-typing {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 80vw;
      margin-top: 2vh;
    }

    .css-typing p {
      border-right: .15em solid lightgray;
      font-size: 7rem;
      white-space: nowrap;
      overflow: hidden;
    }

    .css-typing p:nth-child(1) {
      width: 13em;
      -webkit-animation: type 2s steps(40, end);
      animation: type 2s steps(40, end);
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
    }

    .css-typing p:nth-child(2) {
      width: 11.5em;
      opacity: 0;
      -webkit-animation: type2 2s steps(40, end);
      animation: type2 2s steps(40, end);
      -webkit-animation-delay: 2s;
      animation-delay: 2s;
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
    }

    .css-typing p:nth-child(3) {
      width: 13em;
      opacity:  0;
      -webkit-animation: type3 5s steps(20, end), blink .5s step-end infinite alternate;
      animation: type3 5s steps(20, end), blink .5s step-end infinite alternate;
      -webkit-animation-delay: 4s;
      animation-delay: 4s;
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
    }

}


.row::after {
  content: "";
  clear: both;
  display: table;
}



/* Animations */

@keyframes type {
  0% {
    width: 0;
  }
  99.9% {
    border-right: .15em solid orange;
  }
  100% {
    border: none;
  }
}

@-webkit-keyframes type {
  0% {
    width: 0;
  }
  99.9% {
    border-right: .15em solid orange;
  }
  100% {
    border: none;
  }
}

@keyframes type2 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid lightgray;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type2 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid lightgray;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type3 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}

@-webkit-keyframes type3 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
@-webkit-keyframes blink {
  50% {
    border-color: tranparent;
  }
}

</style>