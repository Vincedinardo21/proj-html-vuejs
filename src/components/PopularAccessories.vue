<template>
    <div class="container-fluid">       
        <div class="row">
            <div class="col-6 img-container-L">
                <div>
                    <div>FIND THE BEST ANIMAL SUPPLIES</div>
                    <h2>Popular accessories</h2>
                    <div class="btn-card"><a href="#">View all toys accessories</a></div>
                </div>        
            </div>

            <div class="col-6 img-container-R">
                <div>
                    <div>FIND THE BEST FOOD</div>
                    <h2>New food arrival</h2>
                    <div class="btn-card"><a href="#">View all food products</a></div>
                </div>       
            </div>
        </div>
        
        <div class="row">
            <div class="col-12 banner">
                <div class="container">
                    <div class="row">
                        <div class="col-12 icon-container">
                            <div>
                                <div><font-awesome-icon icon="fa-solid fa-truck" /></div>
                                <div>Free worldwide deliveries</div>
                            </div>
                            <div>
                                <div><font-awesome-icon icon="fa-solid fa-store" /></div>
                                <div>Fine store near you</div>
                            </div>
                            
                            <div>
                                <div><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
                                <div>Best price guarranteed</div>
                            </div>
                            
                            <div>
                                <div><font-awesome-icon icon="fa-solid fa-credit-card" /></div>
                                <div>All credit card accepted</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'PopularAccessories',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .img-container-L, .img-container-R {
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
        background-size: cover;
        height: 500px;
        color: white;
    }
    .img-container-L{
        background-image: url("../assets/img/banner-8-2x.jpg");
    }
    .img-container-R{
        background-image: url("../assets/img/banner-9-2x.jpg");
    }

    .banner {
        background-image: url("../assets/img/bg-transparent-3.png");
        background-color: #2a382a;
        background-repeat: repeat-x;
        color: white;
    }

    .icon-container{
        height: 350px;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    .btn-card {
            a {
                background-color: white;
                color: black;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
</style>