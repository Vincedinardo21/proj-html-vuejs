<template>
    <div class="container">
        <div class="row">
            <div class="col-12">          
                <div class="news-content">
                    <div>
                        <h2>Join our newsletters</h2>
                        <p>Volutpat vel turpis nulla lorem sed semper. Aliquam sagittis sem libero viverra vehicula nullam ut nisl.</p>
                        <div id="input-area">
                            <span class="btn-email"><input type="email" placeholder="Insert your email..."></span>
                            <span class="btn-card"><a href="#">Subscribe</a></span>
                        </div> 
                    </div>     
                </div>         
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'OurNewsletter',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #input-area{
        margin: 50px 0;
    }
    .news-content{
        height: 400px;
        background-image: url("../assets/img/banner-7-2x-scaled.jpg");
        background-size: cover;

        h2{
            margin: 50px 0;
        }

        div{
            width: 500px;
        }
    }
    .btn-card {
      
      margin: 25px 0;
            a {
                background-color: rgb(61, 111, 66);
                color: white;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
    .btn-email {
      margin: 25px 20px;
            input {  
                height: 37px;        
                background-color: white;
                color: black;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
</style>