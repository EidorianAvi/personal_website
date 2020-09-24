<template>
  <div class="about-page">
    <div class="container">
        <div class="portfolio-image .col-6 .col-s-6">
            <img src="../assets/images/portrait.jpg" alt="Hiking Adventure" class="portrait">
        </div>
        <div class="about-details .col-12 .col-s-12">
            <div class="about-heading">
                <h1>About</h1>
            </div>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus delectus eius, voluptatum impedit et alias consequatur, nisi earum at repellat aliquid velit officiis placeat ipsum assumenda. Totam dolorum ad minima molestias reiciendis impedit earum tenetur dolorem aut neque corrupti mollitia optio, voluptatem officiis? Alias excepturi praesentium qui quisquam modi explicabo consequatur voluptates magnam recusandae exercitationem, tempora cupiditate minus aut ex?
            </p>
            <div class="social-media">
                <ul class="nav-list">
                    <li>
                        <a href="#" class="icon-link">
                            <i class="fa fa-linkedin-square"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="icon-link">
                            <i class="fa fa-github-square"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#" class="icon-link">
                            <i class="fa fa-twitter-square"></i>
                        </a>
                    </li>
                </ul>
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
.about-page {
    /* display: flex; */
    width: 100%;
    height: 100%;
    padding: 5rem;
}


.container {
    /* width: 80%; */
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* transform: translate( -50%, -50%); */
}

.about-heading {
    text-align: center;
    text-transform: uppercase;
    line-height: 0;
    margin-bottom: 8rem;
}

.about-heading h1 {
    font-size: 10rem;
    opacity: .5;
}


.portfolio-image {
    display: flex;
    justify-content: center;
}

.portrait {
    width: 60%;    
}

.about-details {
    flex: 1;
    padding: 5rem;
}

li {
    list-style-type: none;
}

.nav-list{ 
    display: flex;
    justify-content: space-evenly;
}

.social-media {
    margin-top: 5rem;
}

.social-media i{
    font-size: 5rem;
    transition: color 650ms;
    opacity: .9;
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}

@media only screen and (min-width: 992px) {
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
</style>