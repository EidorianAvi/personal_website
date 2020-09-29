<template>
  <div class="about-page">
    <div class="container">
        <div  class="portfolio-image" @click="cycleImage">
            <img 
            :src="require(`../assets/images/${ this.currentImage || 'portrait.jpg' }`)" 
            alt="About images" 
            class="portrait">
            <p>{{ this.currentDescription }}</p>
        </div>
        <div class="about-details">
            <div class="about-heading">
                <h1>About</h1>
            </div>
            <p>
               Welcome to my page, make yourself comfortable. The name is Adrian, and I'm an up and coming Full Stack Software Engineer just looking to live, learn and build. Two things I believe down to my core are 1. there's always room for improvement and 2. Han shot first. In my free time you can likely find me arguing with my dog, watching/reading Star Wars or learning spoken and written languages, i'm currently working on my Spanish and Japanese. I have dreams of traveling far and wide and building bigger and better for myself and the world around me. If you'd like to see more on my personal life click on my mug above. 
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
            <div class="border"></div>
        </div>
    </div>      
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
                {title: 'Riku.jpeg', description: 'This is my little boy Riku'},
                {title: 'travel1.jpg', description: 'I enjoy traveling'},
                {title: 'Family2.jpeg', description: "Family means.."},
                {title: 'Family.jpg', description: "..a lot.."},
                {title: 'Family3.jpg', description: "...to me"},
                {title: 'books.jpg', description: 'I collect Star Wars books and comics'},
                {title: 'Ramen.jpg', description: "... and I'm always up for a bowl of Ramen"},
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

    .portfolio-image {
        height: 40vh;
        width: 100%;
    }

    .portfolio-image img{
        max-height: 40vh;
        width: auto;
        max-width: 80vw;
    }

    .portfolio-image p {
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

  .about-heading h1 {
    font-size: 10rem;
    opacity: .5;
    }
}

.row::after {
  content: "";
  clear: both;
  display: table;
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

.about-heading {
    text-align: center;
    text-transform: uppercase;
}


.portfolio-image {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.portrait {
    width: 60%;    
}


li {
    list-style-type: none;
}


.social-media {
    margin-top: 5rem;
}

.social-media i{
    font-size: 5rem;
    transition: color 650ms;
    opacity: .9;
}

</style>