<template>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <div class="main-text">
                    <h2>Browse by category</h2>
                    <p>Augue purus et, tincidunt condimentum mauris. At nibh rutrum mi in. Nisi, vitae interdum eleifend dui, consequat nulla rhoncus dictum. Viverra.</p>
                </div>     
            </div>

            <!-- Products -->
            <div class="col-12">
                <div class="products-container">
                    <div class="card" v-for="(item, i) in products" :key="i">
                        {{item.text}}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'BrowseBy',
  data(){
    return {
        products : [
            {
                image : "",
                text : "Bed",
                quantity : 1
            },
            {
                image : "",
                text : "Food",
                quantity : 6
            },
            {
                image : "",
                text : "Toys",
                quantity : 6
            },
            {
                image : "",
                text : "Transport",
                quantity : 6
            }
        ]
    }
  } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .main-text {
        text-align: center;
    }
</style>