<template>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <div class="main-text">
                    <h2>Browse by category</h2>
                    <p>Augue purus et, tincidunt condimentum mauris. At nibh rutrum mi in. Nisi, vitae interdum eleifend dui, consequat nulla rhoncus dictum. Viverra.</p>
                </div>     
            </div>

            <!-- Products card-->
            <div class="col-12">
                <div class="products-container">
                    <div class="my-card" v-for="(item, i) in products" :key="i">
                        <img :src="item.image" :alt="item.text">
                        {{item.text}} ({{item.quantity}})
                    </div>
                </div>
            </div>

            <!-- Food card -->
            <div class="col-12">
                <div class="food-container">
                    <div class="food-card" v-for="(item, i) in foods" :key="i">
                        <h2>{{item.text}}</h2>
                        <h5>{{item.type}}</h5>
                        <img :src="item.image" :alt="item.text">
                        <div class="btn-card"><a href="#">Shop {{item.btn}}</a></div>
                    </div>
                </div>
            </div>

            <!-- New arrivals weeckly -->
            <div class="col-12 arrivals-banner">       
                <div class="arrivals-text">
                    <div>FIND THE BEST ANIMAL SUPPLIES</div>
                    <h2>New arrivals weekly</h2>
                    <div class="btn-card"><a href="#">Learn more about us</a></div>
                </div>
            </div>

            <!-- Best sellers -->
            <div class="col-12">
                <div class="seller-container">
                    <div class="text-and-btn">
                        <div>All-time best sellers</div>
                        <div class="btn-card"><a href="#">View all products</a></div>
                    </div> 
                    <h3>Items everyone loves</h3>
                    <div class="items-container">
                        <div class="item-card" v-for="(item, i) in items" :key="i">
                            <img :src="item.image" :alt="item.text">
                            <h5>{{item.text}}</h5>
                            <span class="line">{{item.discount}}</span> <span class="green-text">{{item.price}}</span> 
                        </div>  
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
                image : require("../assets/img/product-9.jpg"),
                text : "Bed",
                quantity : 1
            },
            {
                image : require("../assets/img/product-3.jpg"),
                text : "Food",
                quantity : 6
            },
            {
                image : require("../assets/img/product-2.jpg"),
                text : "Toys",
                quantity : 6
            },
            {
                image : require("../assets/img/product-4.jpg"),
                text : "Transport",
                quantity : 6
            }
        ],

        foods : [
            {
                text : "Kibble",
                type : "Dry dog food",
                image : require("../assets/img/food-transparent-18.png"),
                btn : "dry food"
            },
            {
                text : "Moist",
                type : "Canned dog food",
                image : require("../assets/img/food-transparent-17.png"),
                btn : "moist food"
            },
            {
                text : "Frozen",
                type : "Freez-Died dog food",
                image : require("../assets/img/food-transparent-16.png"),
                btn : "frozen food"
            }
        ],

        items : [
            {
                image : require("../assets/img/product-21.jpg"),
                text : "Transport cage",
                price : "$25.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-20.jpg"),
                text : "Dog leash",
                price : "$25.00",
                discount : ""
            },
            {
                image : require("../assets/img/product-16.jpg"),
                text : "Animal transport cage",
                price : "$25.00",
                discount : "$35.00"
            },
            {
                image : require("../assets/img/product-11.jpg"),
                text : "Colorful cat leash",
                price : "$12.00",
                discount : ""
            }
        ]
    }
  } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .container {
        text-align: center;
    }

    .products-container, .food-container{
        display: flex;
        justify-content: space-between;

        img {
            width: 310px;
        }
    }
    .food-container {
        margin: 20px 0;
    }

    .btn-card {
            a {
                background-color: rgb(61, 111, 66);
                color: white;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
    .food-card {
        background-image: url("../assets/img/bg-transparent-3.png");
        background-color: #2a382a;
        background-repeat: no-repeat;
        padding: 55px;

        &:hover {
            transform: scale(1.05);
        }

        h2 {
            color: white;
        }

        h5 {
            color: #59b742
        }        
    }
    .arrivals-banner {
        height: 500px;
        background-image: url("../assets/img/banner-3-2x-scaled.jpg");
        background-size: cover;

        display: flex;
        justify-content: center;
        align-items: center;
    }

    .text-and-btn {
        display: flex;
        justify-content: space-between;
    }

    .items-container {
        display: flex;
        justify-content: space-between;

        img {
            width: 310px;
        }

        .line {
            text-decoration: line-through;
            color: gray;
        }

        .green-text {
            color: green;
        }
    }

</style>