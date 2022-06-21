<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h2>New products arrival</h2>
                    <div id="latest">Latest product</div>
                    <div class="card-container">
                        <div class="my-card" v-for="(item, i) in newProducts" :key="i">
                            <img :src="item.image" :alt="item.text">
                            <h5>{{item.text}}</h5>
                            <span>{{item.discount}}</span> <span>{{item.price}}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'NewProducts', 
  data(){
    return {
        newProducts : [
            {
                image : require("../assets/img/product-8.jpg"),
                text : "Colored pet bed",
                price : "$18.00 - $26.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-2.jpg"),
                text : "Colorful ball set",
                price : "$29.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-3.jpg"),
                text : "Dog bone",
                price : "$18.00",
                discount : "$29.00"
            },
            {
                image : require("../assets/img/product-4.jpg"),
                text : "Animal transport bag",
                price : "$29.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-5.jpg"),
                text : "Animal transport cage",
                price : "$35.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-10.jpg"),
                text : "Closable cat litter",
                price : "$16.00",
                discount : ""
            },
        ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section{
        padding-bottom: 100px;
        text-align: center;

        h2{
            margin-top: 100px;
        }

        #latest{
            color: green;
            margin-top: 20px;
            margin-bottom: 50px;
        }
        
    }
    .card-container{
        display: flex;
        flex-wrap: wrap;

        .my-card {
            flex-basis: calc(100% / 3);
        }
        img {
            width: 410px;
        }
    }
</style>