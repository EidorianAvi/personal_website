<template>
    <div class="col-12 portfolio" id="portfolio"
        data-aos="fade-right"
        data-aos-delay="300"
        data-aos-duration="1500"
        data-aos-easing="ease-in-out"
    >
        <div class="container">
            <div class="section-heading">
                <h1>Portfolio</h1>
            </div>
            <div class="recent-projects">
                <h1>Recent Projects</h1>
            </div>
            <div class="demo-videos">
                <div class="portfolio-item">
                    <h2>smallTalk</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/aZMOCxSa3Yg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <p>smallTalk is the middleman to interest and hobby driven conversation. Sometimes it's difficult to  <span class="see-more-1" @click="expandDescription(1)">...see more</span><span class="more-1">spark up a conversation about topics that are near and dear to you but have nobody to relate with. That's where smallTalk comes in it's the one stop shop to meet, converse, and connect with likeminded individuals. Technologies used were: Flutter, Dart, Firebase, and Firestore. </span><span class="see-less-1" @click="expandDescription(1)">...see less</span></p>
                </div>
                <div class="portfolio-item">
                    <h2>theRack</h2>
                    <div class="iframe-container">
                        <iframe width="560"  height="315" src="https://www.youtube.com/embed/5GngnwWPQiI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <p>If you're anything like me you love a good pair of sneakers but have a hard time picking out the perfect <span class="see-more-2" @click="expandDescription(2)">...see more</span><span class="more-2">pair and that's what theRack was created for. Select from hundreds of shoes in the catalogue and narrow it down to the perfect pair. Technologies used were: React, JavaScript, Ruby on Rails, and JWT.</span><span class="see-less-2" @click="expandDescription(2)">...see less</span></p>
                </div>
                <div class="portfolio-item">
                    <h2>Jedi Archives</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/XglSvmMSHPk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <p>A common problem we all face is that our Star Wars collection is just getting larger by the day and it's <span class="see-more-3" @click="expandDescription(3)">...see more</span><span class="more-3">getting difficult to keep track. The Jedi Archives were created to have one place to store all Novels and Graphic Novels for collection management. Technologies used were: JavaScript, Ruby on Rails, CSS3, HTML5.</span><span class="see-less-3" @click="expandDescription(3)">...see less</span></p>
                </div>
            </div>
        <div class="border"></div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        expandDescription(number) {
            
            let seeMore = document.querySelector(`.see-more-${number}`);
            let moreText = document.querySelector(`.more-${number}`);
            let seeLess = document.querySelector(`.see-less-${number}`);

            if (seeMore.style.display === "none") {
                seeMore.style.display = "inline";
                moreText.style.display = "none";
                seeLess.style.display = "none";
           } else {
                seeMore.style.display = "none";
                moreText.style.display = "inline";
                seeLess.style.display = "inline";
            }
        },
    }

}
</script>

<style scoped>

/* For mobile phones: */
@media only screen and (max-width: 600px) {
    [class*="col-"] {
    width: 100%;
    }

    .portfolio {
        margin-top: 8rem;
        max-width: 100%;
        height: auto;
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

    .see-more-1, .see-more-2, .see-more-3 {
        display: inline;
        color: grey;
        font-weight: 600;
    }

    .more-1, .more-2, .more-3 {
        display: none;
    }

    .see-less-1, .see-less-2, .see-less-3 {
        display: none;
        color: grey;
        font-weight: 600;
    }

    .border {
        margin-top: 15vh;
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
  
    .portfolio {
          height: 100vh;
    }

    .container {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        height: 100vh;
    }

    .section-heading h1 {
        margin-top: 10vh;
        font-size: 30rem;
        text-align: center;
        opacity: .5;
    }

    .recent-projects {
        margin-left: 4vw;
        margin-bottom: 10vh;
        width: 30%;
        border-bottom: 1px lightgrey solid;
    }

    .recent-projects h1 {
        font-size: 10rem;
        font-weight: 300;
        opacity: .7;
    }

    .demo-videos {
        width: 100vw;
        display: flex;
        justify-content: space-evenly;
    }

    .demo-videos h2 {
        font-size: 5rem;
        padding-bottom: 2vh;
    }

    .iframe-container iframe{
        height: 25vh;
        width: 25vw;
    }

    p {
        padding-top: 1vh;
        width: 25vw;
        font-size: 4rem;
    }

    .see-more-1, .see-more-2, .see-more-3 {
        display: inline;
        color: grey;
        font-weight: 600;
    }

    .more-1, .more-2, .more-3 {
        display: none;
    }

    .see-less-1, .see-less-2, .see-less-3 {
        display: none;
        color: grey;
        font-weight: 600;
    }

    .border {
        margin-top: 20vh;
        margin-left: 35vw;
        width: 30vw;
        border-bottom: 1px solid lightgrey;
    }

}

.row::after {
  content: "";
  clear: both;
  display: table;
}





</style>