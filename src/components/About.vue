<template>
  <div class="about-page">
    <div class="container">
        <div class="portfolio-image">
            <img src="../assets/images/portrait.jpg" alt="Hiking Adventure" class="portrait">
        </div>
        <div class="about-details">
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
    display: flex;
    width: 100%;
    padding: 5rem;

}


.container {
    /* width: 80%; */
    display: flex;
    align-items: center;
    justify-content: space-between;
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
</style>