<template>
    <footer>
      <div class="container">
        <div class="row">
          <div class="col-12">
            <!-- <h2>Footer</h2> -->
            <div class="my-content">

              <div class="logo">
                <img src="../assets/img/mobile-light-pet-logo-2x.png" alt="">
                <div>1234 Avada Avenue Avadaville</div>
                <div>Info@your-company.com</div>
                <div>Call us: (1) 234 5678</div>
              </div>

              <div class="Shop-list">
                <ul>
                  <li><h5>Shop by brand</h5></li>
                  <li><a href="#">Bed</a></li>
                  <li><a href="#">Food</a></li>
                  <li><a href="#">Toys</a></li>
                  <li><a href="#">Transport</a></li>
                </ul>
              </div>

              <div class="Useful-list">
                <ul>
                  <li><h5>Useful links</h5></li>
                  <li><a href="#">My account</a></li>
                  <li><a href="#">Orders</a></li>
                  <li><a href="#">Checkout</a></li>
                  <li><a href="#">Cart</a></li>
                </ul> 
              </div>

              <div class="subscribe">
                <h5>Subscribe to our newsletter</h5>
                <div class="btn-email"><input type="email" placeholder="Insert your email..."></div>
                <div class="btn-card"><a href="#">Subscribe</a></div>
              </div>
            </div>
          </div>

          <div class="col-12">
            <div class="down-footer">
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Shop</a></li>
              </ul>

              <div class="icons">
                <font-awesome-icon icon="fa-brands fa-facebook-f" />
                <font-awesome-icon icon="fa-brands fa-twitter" />
                <font-awesome-icon icon="fa-brands fa-instagram" />
                <font-awesome-icon icon="fa-brands fa-youtube" />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="copyright">
        <font-awesome-icon icon="fa-regular fa-copyright" /><span>Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All rights Reserved | Powered by WordPress</span> 
      </div>
    </footer>
</template>

<script>
export default {
  name: 'MyFooter',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer{
      .copyright{
        background-color: black;
        height: 60px;
        display: flex;
        justify-content: center;
        align-items: center;

        span{
          margin-left: 5px;
        }
      }
      a {
        color: white;
        text-decoration: none;
      }

      li{
        list-style-type: none;
        margin: 30px 0;
      }
      padding-top: 100px;
      color: white;
      background-color: #2a382a;

      img{
        width: 200px;
        margin: 30px 0;
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
      margin: 25px 0;
            input {          
                background-color: white;
                color: black;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }

    .subscribe{
      background-image: url("../assets/img/bg-transparent-3.png");
      background-size: 350px;
      background-repeat: repeat-x;
      background-color: rgb(38, 66, 41);
      width: 300px;
      border-radius: 5px;
      padding: 30px;
    }

    .my-content {
      padding-bottom: 60px;
      display: flex;
      justify-content: space-between;
    }

    .down-footer{
      padding-top: 40px;
      border-top: 1px solid gray;
      text-align: center;
      ul{
        li{
          list-style-type: none;
          display: inline-block;
          margin: 0 20px;
          a{
            color: gray;
            text-decoration: none;
          }
        }
      }
      [class*="fa-"]{
        margin: 10px;
      }
    }
    
</style>
