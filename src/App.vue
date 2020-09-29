<template>
  <div id="app">
    <!-- <SideNavigator /> -->
    <Hero />
    <About />
    <Portfolio /> 
    <Blogs /> 
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Hero from './components/Hero';
import About from './components/About';
import Portfolio from './components/Portfolio';
import Blogs from './components/Blogs';
import Contact from './components/Contact';
import Footer from './components/Footer';
// import SideNavigator from './components/SideNavigator';

export default {
  name: 'app',
  components: {
    Hero,
    About,
    Portfolio,
    Blogs,
    Contact,
    Footer
    // SideNavigator,
  }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
}

html {
  font-family: 'Epilogue', sans-serif;
  font-size: 10px;
  color: #eee;
  max-width: 100%;
}

body {
  max-width: 100%;
  height: 100%;
  background: url('./assets/images/background2.jpg') no-repeat center center fixed;
  background-size: 100% 100%;
}

a {
  text-decoration: none;
  color: #eee;
}

p {
  /* font-size: 1.8rem; */
  font-weight: 300;
}

img {
  width: 100%;
}


</style>
