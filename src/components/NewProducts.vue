<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h2>New products arrival</h2>
                    <div id="latest">Latest product</div>
                    <div class="card-container">
                        <a href="#" class="my-card" v-for="(item, i) in newProducts" :key="i">
                            <div id="myimg">
                                <img :src="item.image" :alt="item.text">
                            </div>
                            
                            <h5>{{item.text}}</h5>
                            <span id="discount">{{item.discount}}</span> <span id="price">{{item.price}}</span>
                            <div class="cart">
                                <font-awesome-icon icon="fa-solid fa-square-check" />
                                <div>VIEW CART</div> 
                            </div>
                        </a>
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
        a {
        text-decoration: none;
        color: black;
         }
        padding-bottom: 100px;
        text-align: center;

        h2{
            margin-top: 100px;
        }

        #latest{
            color: rgb(61, 111, 66);
            margin-top: 20px;
            margin-bottom: 50px;
        }
        
    }
    .card-container{
        display: flex;
        flex-wrap: wrap;

        .my-card {
            position: relative;
            .cart{
                color: white;
                position: absolute;
                left: 165px;
                top: 170px;
                display: none;
                .fa-square-check{
                    font-size: 40px;
                    border: 1px solid black;
                    border-radius: 50px;
                    background-color: black;
                    padding: 10px 13px;
                }
            }
            #myimg{
                background-color: black;
                margin: 20px 0;
                width: 410px;
            }
            flex-basis: calc(100% / 3);
            &:hover{
                .cart{
                    display: block;
                }
                img{
                    opacity: 0.5;
                }
            }
        }
        img {
            width: 100%;
            
        }
        #discount {
            text-decoration: line-through;
            font-size: 12px;
        }
        #price {
            color: rgb(61, 111, 66);
        }
    }
</style>