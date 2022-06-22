<template>
    <div class="container-fluid">       
        <div class="row">
            <div class="col-6 img-container-L">
                <div class="bg-fade">
                    <div>
                        <div>FIND THE BEST ANIMAL SUPPLIES</div>
                        <h2>Popular accessories</h2>
                        <div class="btn-card"><a href="#">View all toys accessories</a></div>
                    </div> 
                </div>       
            </div>

            <div class="col-6 img-container-R">
                <div class="bg-fade">
                    <div>
                        <div>FIND THE BEST FOOD</div>
                        <h2>New food arrival</h2>
                        <div class="btn-card"><a href="#">View all food products</a></div>
                    </div>
                </div>       
            </div>
        </div>
        
        <div class="row">
            <div class="col-12 banner">
                <div class="container">
                    <div class="row">
                        <div class="col-12 icon-container">
                            <a href="#">
                                <div><font-awesome-icon icon="fa-solid fa-truck" /></div>
                                <div class="colored">Free worldwide deliveries</div>
                            </a>
                            <a href="#">
                                <div><font-awesome-icon icon="fa-solid fa-store" /></div>
                                <div class="colored">Find store near you</div>
                            </a>
                            
                            <a href="#">
                                <div><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
                                <div class="colored">Best price guarranteed</div>
                            </a>
                            
                            <a href="#">
                                <div><font-awesome-icon icon="fa-solid fa-credit-card" /></div>
                                <div class="colored">All credit card accepted</div>
                            </a>
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

    a{
        color: white;
        text-decoration: none;
    }

    .bg-fade{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgba(0,0,0,0.3);
    }

    .colored {
        color: rgb(156, 165, 159);
    }

    h2{
        margin-top: 20px;
        margin-bottom: 35px;
    }
    .img-container-L, .img-container-R {
        padding: 0;
        text-align: center;
        
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

                &:hover {
                    background-color: rgb(61, 111, 66);
                    color: white;
                }
            }
        }
</style>