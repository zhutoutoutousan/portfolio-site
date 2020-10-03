<template>
  <div id="app">
    <contact-component></contact-component>
    <brand-component></brand-component>
    <navigation-component></navigation-component>
    <introduction-component></introduction-component>
    <router-view/>
    <footer-component></footer-component>
  </div>
</template>

<script>
import ContactComponent from './components/ContactComponent'
import BrandComponent from './components/BrandComponent'
import NavigationComponent from './components/NavigationComponent'
import FooterComponent from './components/FooterComponent'
import IntroductionComponent from './components/IntroductionComponent'


export default {
  components: {
    ContactComponent, 
    BrandComponent, 
    NavigationComponent, 
    FooterComponent, 
    IntroductionComponent}
}
</script>

<style lang="scss">
#app {
  min-height: 100%;
  padding: 1.5rem;
  background-color: $color-secondary;
  user-select: none;
  position: relative;
}

</style>
