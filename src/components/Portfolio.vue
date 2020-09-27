<template>
    <div class="portfolio" id="portfolio">
        <div class="container">
            <div class="section-heading">
                <h1>Portfolio</h1>
            </div>
            <div class="demo-videos">
                <div class="portfolio-item">
                    <div class="recent-projects">
                        <h1>Recent Projects</h1>
                    </div>
                    <h2>smallTalk</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/aZMOCxSa3Yg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="portfolio-item">
                    <h2>theRack</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/5GngnwWPQiI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="portfolio-item">
                    <h2>Jedi Archives</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/XglSvmMSHPk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
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

    .section-heading h1 {
        font-size: 6rem;
        opacity: .5;
        text-align: center;
        margin-bottom: 2rem;
    }

    .recent-projects {
        margin-left: 4rem;
        width: 60%;
        border-bottom: 1px lightgrey solid;
    }

    .recent-projects h1 {
        font-size: 2rem;
        font-weight: 300;
        opacity: .8;
        text-align: left;
        /* text-decoration: underline; */
    }

    .demo-videos h2 {
        font-size: 1.5rem;
        text-align: left;
        padding: 4rem;
        font-style: italic;
        color: lightgray;
    }

    .iframe-container {
        display: flex;
        justify-content: center;
    }

    .iframe-container iframe{
        max-width: 80%;
        height: auto;
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

  .section-heading h1 {
    font-size: 1rem;
    opacity: .5;
    }

}

.row::after {
  content: "";
  clear: both;
  display: table;
}

.portfolio {
    margin-top: 10rem;
    max-width: 100%;
    height: 110vh;
}



</style>