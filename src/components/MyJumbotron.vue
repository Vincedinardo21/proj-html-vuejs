<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 jumbo-up-back">
                <!-- Jumbo up -->
                <div class="container">
                    <div class="row">      
                        <div class="col-12 jumbo-up">
                            <div><font-awesome-icon icon="fa-solid fa-book-open" /><b> International</b> Shipping Services</div>
                            <div><font-awesome-icon icon="fa-regular fa-clock" /> See our <b>store hours</b> and services</div>
                            <div><font-awesome-icon icon="fa-solid fa-check" /> We price match to give you the <b>best deals</b></div>
                        </div>
                    </div>
                </div>
            </div>
            
            

            <!-- Image Background -->
            <div class="col-12 jumbo-banner">
                <div class="jumbo-fade">
                    <div class="container">
                        <div class="row">
                            <div class="col-6 col-learn">
                                <div>
                                    <span>FIND THE BEST ANIMAL SUPPLIES</span>
                                    <h2>We know animals are a part of your family, let us help take care of them.</h2>
                                    <div class="btn-learn"><a href="#">Learn more about us</a></div>
                                </div>                        
                            </div>
                        </div>
                    </div>
                </div>               
            </div>
            
            <!-- Jumbo down -->
            <div class="col-12 jumbo-down">
                <div>
                    <img src="../assets/img/food-transparent-5.png" alt="food">
                    <span>Get $25 OFF your first purchase of our homemade pet food!</span> 
                    <a href="#">Visit the shop</a>
                </div>
                
            </div>
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
    .jumbo-fade{
        background-color: rgba(0,0,0,0.3);       
    }

    .jumbo-up-back {
        background-image: url("../assets/img/bg-transparent-3.png");
        background-color: #2a382a;
        color: white;
    }
    .jumbo-up {
        height: 60px;     
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
    .jumbo-banner {
        height: 760px;
        background-image: url("../assets/img/banner-5-2x-scaled.jpg");    
        background-repeat: no-repeat;
        background-size:cover;
        background-position: center;

        .col-learn {
            height: 760px;
            display: flex;
            align-items: center;

            div {
                color: white;

                h2 {
                    font-size: 55px;
                    margin: 45px 0;
                }
            }
        }
        .btn-learn {
            a {
                background-color: white;
                color: black;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;

                &:hover {
                    background-color: rgb(61, 111, 66);
                    color: white;
                }
            }
        }
    }
    .jumbo-down {
        background-image: url("../assets/img/bg-transparent-3.png");
        background-color: #2a382a;
        color: white;

        div {
            display: flex;
            justify-content: center;
            align-items: center;

            a {
                color: rgb(188, 194, 189);
            }

            span {
                margin: 0 50px;
            }
        }

        img {
            width: 200px;
        }
    }
</style>
