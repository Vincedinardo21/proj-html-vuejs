<template>
    <header>

      <!-- Logo & Searchbar Area -->
      <section class="logo-container">
        <div class="container">
          <div class="row">
            <div class="col-12 area-flex">
              <!-- Logo -->
              <img src="../assets/img/dark-pet-logo.png" alt="Logo">
              <!-- Searchbar -->
              <div class="my-searchbar">
                <a href="#"><font-awesome-icon icon="fa-solid fa-magnifying-glass" /></a>      
                <input type="text" placeholder="Search...">
              </div>
              
              <!-- Questions -->
              <div><b>Questions?</b> Call us : 1.800.123.4567</div>
              <!-- Accedi -->
              <div class="icons">
                <a href="#"><font-awesome-icon icon="fa-solid fa-box-archive" /></a>
                <a href="#"><font-awesome-icon icon="fa-regular fa-user" /></a>        
              </div>
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
                <li v-for="(item, i) in navBar" :key="i"><a :href="item.link">
                  {{item.text}}
                  <font-awesome-icon :icon="item.arrow" />
                </a></li>
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
          link : "#",
          arrow : "fa-solid fa-chevron-down"
        },
        {
          text : "Shop",
          link : "#",
          arrow : "fa-solid fa-chevron-down"
        },
        {
          text : "About",
          link : "#",
          arrow : ""
        },
        {
          text : "Blog",
          link : "#",
          arrow : ""
        },
        {
          text : "Contact",
          link : "#",
          arrow : ""
        },
        {
          text : "Shop by brand",
          link : "#",
          arrow : "fa-solid fa-chevron-down"
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .container {
    ul{
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      
      li{
        list-style-type: none;
        margin: 0 30px;

        a{
          text-decoration: none;
          color: gray;
        }
      }
    }
  }
  .area-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .logo-container{
    // Debug
    // background-color: aqua;
    padding: 20px 0;
    border-bottom: 1px solid gray;

    .my-searchbar {
      width: 320px;
      padding: 7px;
      
      border-radius: 20px;
      background-color:rgb(243, 243, 243);
    }

    input {
      border: none;
      background-color:rgb(243, 243, 243);
    }

    [class*="fa-"]{
      margin: 0 10px;
      color: black;
    }
  }
</style>
