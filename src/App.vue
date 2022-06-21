<template>
  <div id="app">
      <!-- Header -->
      <MyHeader/>

      <!-- Main -->
      <main>
        <!-- Jumbotron -->
        <MyJumbotron/>
        <!-- Browse by category -->
        <BrowseBy/>
        <!-- Users testimonials -->
        <UserTestimonials/>
        <OurNewsletter/>
        <!-- Get tips -->
        <GetTips/>
        <!-- Accessories -->
        <PopularAccessories/>
        <!-- New products arrivals -->
        <NewProducts/>
      </main>

      <!-- Footer -->
      <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbotron from './components/MyJumbotron.vue'
import MyFooter from './components/MyFooter.vue'
import BrowseBy from './components/BrowseBy.vue'
import UserTestimonials from './components/UserTestimonials.vue'
import OurNewsletter from './components/OurNewsletter.vue'
import GetTips from './components/GetTips.vue'
import PopularAccessories from './components/PopularAccessories.vue'
import NewProducts from './components/NewProducts.vue'



export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    MyFooter,
    BrowseBy,
    UserTestimonials,
    OurNewsletter,
    GetTips,
    PopularAccessories,
    NewProducts
}
}
</script>

<style lang="scss">
// Reset
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

[class*="col-"] {
  // Debug
  //border: 1px solid black;
  min-height: 50px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  //margin-top: 60px;
}
</style>
