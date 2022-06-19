<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 jumbo-up"></div>
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
    .jumbo-fade{
        background-color: rgba(0,0,0,0.3);
        
    }
    .jumbo-up {
        background-color: aquamarine;
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
</style>
