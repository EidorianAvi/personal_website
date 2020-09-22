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
  background: url('./assets/images/background.jpg') no-repeat center fixed;
}
</style>
