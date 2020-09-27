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
                    <p>smallTalk is the middleman to interest and hobby driven conversation. Sometimes it's difficult to  <span id="dots">...see more</span><span id="more">erisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta.</span></p>
                </div>
                <div class="portfolio-item">
                    <h2>theRack</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/5GngnwWPQiI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas vitae scel<span id="dots">...see more</span><span id="more">erisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta.</span></p>
                </div>
                <div class="portfolio-item">
                    <h2>Jedi Archives</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/XglSvmMSHPk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas vitae scel<span id="dots">...see more</span><span id="more">erisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta.</span></p>
                </div>
            </div>
        </div>
        <div class="border"></div>
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
        width: 50%;
        border-bottom: 1px lightgrey solid;
    }

    .recent-projects h1 {
        font-size: 1.5rem;
        font-weight: 300;
        opacity: .8;
        text-align: left;
        /* text-decoration: underline; */
    }

    .demo-videos h2 {
        font-size: 1.5rem;
        text-align: left;
        padding-top: 3rem;
        padding-left: 4.4rem;
        font-style: italic;
        color: lightgray;
    }

    .iframe-container {
        display: flex;
        justify-content: center;
    }

    .iframe-container iframe{
        max-width: 80vw;
        height: auto;
    }

    p {
        margin-top: 1vh;
        margin-left: 10vw;
        max-width: 80vw;
        font-size: 1.3rem;
    }


    #more {
        display: none;
    }

    .border {
        margin-top: 16vh;
        margin-left: 35vw;
        width: 30vw;
        border-bottom: 1px solid lightgrey;
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