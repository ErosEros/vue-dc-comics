<template>
  <div id="app">
  <HeaderComponent />
  <SectionContent :cards='dates' />
  <SecondSection />
  <FirstFooter />
  <SecondFooter />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import SecondSection from './components/SecondSection.vue';
import FirstFooter from './components/FirstFooter.vue';
import SecondFooter from './components/SecondFooter.vue';
import SectionContent from './components/SectionContent.vue';
import {dates} from './data/data.js'


export default {
  name: 'App',
  data(){
    return {dates}
  },
  components: {
    HeaderComponent,
    SecondSection,
    FirstFooter,
    SecondFooter,
    SectionContent
}
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
