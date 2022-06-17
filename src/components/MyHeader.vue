<template>
    <header>
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
    </header>
</template>

<script>
export default {
  name: 'MyHeader',
  
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
