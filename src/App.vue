<template>
  <div id="app">
    <SideNavigator />
    <About />
    <Portfolio />  
  </div>
</template>

<script>
import SideNavigator from './components/SideNavigator';
import About from './components/About';
import Portfolio from './components/Portfolio';

export default {
  name: 'app',
  components: {
    SideNavigator,
    About,
    Portfolio
  }
}
</script>

<style>

</style>
