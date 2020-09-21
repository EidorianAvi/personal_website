<template>
  <div id="app">
    <SideNavigator />
    <About /> 
  </div>
</template>

<script>
import SideNavigator from './components/SideNavigator'
import About from './components/About'
export default {
  name: 'app',
  components: {
    SideNavigator,
    About,
  }
}
</script>

<style>

</style>
