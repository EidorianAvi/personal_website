<template>
  <div id="app">
    <SideNavigator />
    <Hero />
    <About />
    <Portfolio /> 
    <Blogs /> 
    <Contact />
  </div>
</template>

<script>
import Hero from './components/Hero';
import About from './components/About';
import Portfolio from './components/Portfolio';
import Blogs from './components/Blogs';
import Contact from './components/Contact';
import SideNavigator from './components/SideNavigator';

export default {
  name: 'app',
  components: {
    Hero,
    About,
    Portfolio,
    Blogs,
    Contact,
    SideNavigator,
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 10px;
  font-family: 'Roboto', sans-serif;
  color: #eee;
}

body {
  width: 100%;
  height: 100%;
  background: url('./assets/images/background.jpg') no-repeat center center fixed;
  background-size: cover;
}

a {
  text-decoration: none;
  color: #eee;
}

p {
  font-size: 1.8rem;
  font-weight: 300;
}

img {
  width: 100%;
}

/* For mobile phones: */
[class*="col-"] {
  width: 100%;
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
