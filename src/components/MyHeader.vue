<template>
    <header>

      <!-- Logo & Searchbar Area -->
      <section class="logo-container">
        <div class="container">
          <div class="row">
            <div class="col-12">
              <!-- Logo -->
              <img src="../assets/img/dark-pet-logo.png" alt="Logo">
              <!-- Searchbar -->
              <input type="text" placeholder="Search...">
              <!-- Questions -->
              <div>Questions? Call us: 1.800.123.4567</div>
              <!-- Accedi -->
              <div>Icone...</div>
            </div>
          </div>            
        </div>
      </section> 
      
      <!-- Nav Area -->
      <nav>
        <div class="container">
          <div class="row">
            <div class="col-12">
              <ul>
                <li v-for="(item, i) in navBar" :key="i"><a :href="item.link">{{item.text}}</a></li>
              </ul>
            </div>
          </div>
        </div>
      </nav>

    </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data(){
    return{
      navBar : [
        {
          text : "Home",
          link : "https://bootstrap-vue.org/docs",
        },
        {
          text : "Shop",
          link : "#",
        },
        {
          text : "About",
          link : "#",
        },
        {
          text : "Blog",
          link : "#",
        },
        {
          text : "Contact",
          link : "#",
        },
        {
          text : "Shop by brand",
          link : "#",
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .logo-container{
    // Debug
    background-color: aqua;
    border-bottom: 1px solid gray;
  }
</style>
