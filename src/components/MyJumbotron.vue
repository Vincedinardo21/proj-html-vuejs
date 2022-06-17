<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 jumbo-up"></div>
            <!-- Image Background -->
            <div class="col-12 jumbo-banner"></div>
            <div class="col-12"></div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'MyJumbotron',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .jumbo-up {
        background-color: aquamarine;
    }
    .jumbo-banner {
        height: 760px;
        background-image: url("../assets/img/banner-5-2x-scaled.jpg");
        background-repeat: no-repeat;
        background-size:cover;
        background-position: center;
    }
</style>
