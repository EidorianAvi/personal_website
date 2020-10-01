<template>
  <div class="col-12 about-page">
    <div class="col-12 container">
        <div class="col-5 portfolio-image" >
            <div
            class="image-box"
            @click="cycleImage"
            data-aos="zoom-out"
            data-aos-delay="300"
            data-aos-duration="1500"
            data-aos-easing="ease-in-out"
            data-aos-once="false"
            >
                <img 
                :src="require(`../assets/images/${ this.currentImage || 'portrait.jpg' }`)" 
                alt="About images" 
                class="portrait">
                <p>{{ this.currentDescription }}</p>
            </div>
            
        </div>
        <div 
        class="col-5 about-details"
        data-aos="zoom-in"
        data-aos-delay="300"
        data-aos-duration="1500"
        data-aos-easing="ease-in-out"
        data-aos-once="false"
        >
            <div class="about-heading">
                <h1>About</h1>
            </div>
            <p>
               Welcome to my page, make yourself comfortable. The name is Adrian, and I'm an up and coming Full Stack Software Engineer just looking to live, learn and build. Two things I believe down to my core are 1. there's always room for improvement and 2. Han shot first. In my free time you can likely find me arguing with my dog, watching/reading Star Wars or learning spoken and written languages, i'm currently working on my Spanish and Japanese. I have dreams of traveling far and wide and building bigger and better for myself and the world around me. If you'd like to see more on my personal life click on my mug <span class="above">above</span><span class="left">to the left</span>. 
            </p>
            <div class="social-media">
                <ul class="nav-list">
                    <li>
                        <a href="https://www.linkedin.com/in/eidorianavi/" class="icon-link">
                            <i class="fa fa-linkedin-square"></i>
                        </a>
                    </li>
                    <li>
                        <a href="https://github.com/EidorianAvi" class="icon-link">
                            <i class="fa fa-github-square"></i>
                        </a>
                    </li>
                    <li>
                        <a href="https://twitter.com/EidorianAvi" class="icon-link">
                            <i class="fa fa-twitter-square"></i>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>      
     <div class="border"></div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            n: 0,
            currentImage: "",
            currentDescription: "", 
            aboutImages: [
                {title: 'portrait.jpg', description: ''},
                {title: 'Barbie.jpg', description: 'I have a lovely lady, Barbie'},
                {title: 'Riku2.jpeg', description: 'This is my little boy Riku'},
                {title: 'travel1.jpg', description: 'I enjoy traveling'},
                {title: 'Family2.jpeg', description: "Family means.."},
                {title: 'Family.jpg', description: "..a lot.."},
                {title: 'Family3.jpg', description: "...to me"},
                {title: 'books.jpg', description: 'I collect Star Wars books and comics'},
                {title: 'Ramen2.jpg', description: "... and I'm always up for a bowl of Ramen"},
            ],
        }
    },
    methods: {
        cycleImage() {
            if(this.n == this.aboutImages.length - 1) {
                this.n = 0;
            } else {
                this.n+=1;
            }

            this.currentImage = this.aboutImages[this.n].title;
            this.currentDescription = this.aboutImages[this.n].description;
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

    .about-page {
        margin-top: 5rem;
        max-width: 100%;
        height: 110vh;
    }

    .container {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }

    .image-box {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .portfolio-image {
        height: 40vh;
        width: 80%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    .portfolio-image img{
        max-width: 80%;
        max-height: 90%; 
    }

    .portfolio-image p {
        text-align: center;
        padding-top: 1rem;
        font-size: 1.3rem;
    }

    .about-heading h1 {
        font-size: 6rem;
        opacity: .5;
        margin-top: 4rem;
    }



    .about-details p { 
        font-size: 1.5rem;
        max-width: 100%;
        padding: 2rem;
        line-height: 2rem;
    }

    .above {
        display: inline;
    }

    .left {
        display: none;
    }

    .social-media {
        width: 100%;
        margin-bottom: 6rem;
    }
    
    .nav-list{ 
        display: flex;
        justify-content: space-evenly;
        opacity: .8;
    }


    .border {
        margin-left: 35vw;
        width: 30vw;
        border-bottom: 1px solid lightgrey;
    }

    .social-media i{
        font-size: 5rem;
        transition: color 650ms;
        opacity: .9;
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

    .container {
        overflow: hidden;
        height: 100vh;
        display: flex;
        justify-content: center;
    }

    .portfolio-image {
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .image-box {
        width: 30vw;
        height: 70vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }


    .portfolio-image img {
        width: 100%;
        max-height: 100%;
        cursor: pointer;
    }


    .portfolio-image p {
        overflow: hidden;
        text-align: center;
        padding-top: 3rem;
        font-size: 7rem;
        opacity: .9;
    }

    .about-details {
        display: flex;
        flex-flow: column wrap;
        align-items: center;
        justify-content: center;
        height: 100%;
    }

    .about-heading h1 {
        font-size: 30rem;
        opacity: .5;
        padding-bottom: 3rem;
    }

    .about-details p {
        font-size: 7rem;
        line-height: 1.4;
        padding-bottom: 3vh;
    }

    .social-media {
        width: 100%;
    }
    
    .about-details ul {
        display: flex;
        justify-content: space-evenly;
    }

    .about-details i {
        font-size: 16rem;
    }

    .above {
        display: none;
    }

    .left {
        display: inline;
    }
    
    .border {
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


.about-heading {
    text-align: center;
    text-transform: uppercase;
}


li {
    list-style-type: none;
}


.social-media {
    margin-top: 5rem;
}



</style>