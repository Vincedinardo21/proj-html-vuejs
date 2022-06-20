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
                    <div class="card" v-for="(item, i) in products" :key="i">
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

        .btn-card {
            a {
                background-color: rgb(61, 111, 66);
                color: white;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
    }
</style>