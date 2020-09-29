<template>
    <div class="blogs" id="blogs"
            data-aos="zoom-out"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
            data-aos-easing="ease-in-out"
            >
        <div class="container">
            <div class="section-heading">
                <h1>Blog Posts</h1>
                <ul>
                    <li v-for="blog in blogs" v-bind:key=blog.id><a v-bind:href="blog.link">{{ blog.title }}</a></li>
                </ul>
            </div>
        </div>
        <div class="border"></div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            blogs: [
                { id: 1, title: 'Enumeration in Ruby', link: 'https://dev.to/eidorianavi/enumeration-in-ruby-2ooi'},
                { id: 2, title: 'Functions and the Single Responsibility Principle', link: 'https://dev.to/eidorianavi/functions-and-the-single-responsibility-principle-48ae'},
                { id: 3, title: 'querySelector vs. getElementById', link: 'https://dev.to/eidorianavi/queryselector-vs-getelementbyid-gm1'},
                { id: 4, title: 'Modular JavaScript: An Inrto to Import and Export', link: 'https://dev.to/eidorianavi/modular-javascript-an-intro-to-import-and-export-2khi'},
                { id: 5, title: 'My time at a coding bootcamp', link: 'https://medium.com/@reneavila1993/my-time-at-a-coding-boot-camp-40238c7a8b0c'},
            ]
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

    .blogs {
        display: flex;
        flex-direction: column;
        max-width: 100%;
        height: 60vh;
    }

    .container {
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .section-heading h1 {
        font-size: 5rem;
        opacity: .5;
        text-align: center;
    }

    .banner-text h6 {
        font-size: 1.75rem;
    }

    ul {
        width: 80vw;
    }

    li {
        font-size: 1.5rem;
        padding-top: 2rem;
        padding-left: 1rem;
        font-style: italic;
        text-decoration-line: underline;
        opacity: .7;
        font-weight: 300;
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
}

.row::after {
  content: "";
  clear: both;
  display: table;
}


</style>