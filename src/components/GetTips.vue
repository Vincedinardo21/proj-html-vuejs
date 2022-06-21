<template>
    <section>
      <div class="container">
        <div class="row">
          <div class="col-12">
            <h2>Get the best tips & tricks</h2>
            <div id="recent">Recent articles</div>
            <div class="card-container">
              <div class="my-card" v-for="(item, i) in tips" :key="i">
                <img :src="item.image" :alt="item.text">
                <div>{{item.text}}</div>
                <div id="data">{{item.data}}</div>
              </div>
            </div>
            <div class="btn-card"><a href="#">Read all articles</a></div>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'GetTips',
  data(){
    return {
      tips : [
        {
          image : require("../assets/img/blog-1.jpg"),
          text : "How to 'loose leash walk' your dog",
          data : "April 21st, 2020"
        },
        {
          image : require("../assets/img/blog-2.jpg"),
          text : "Stop cats from scratching forniture",
          data : "April 19th, 2020"
        },
        {
          image : require("../assets/img/blog-3.jpg"),
          text : "Where to buy the best pet food",
          data : "April 18th, 2020"
        },
        {
          image : require("../assets/img/blog-4.jpg"),
          text : "Proper care for your pet toys",
          data : "April 17th, 2020"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    h2, #recent {
      text-align: center;
      margin: 30px 0;
    }


    #recent{
      color: green;
    }
    .card-container{
        display: flex;
        justify-content: space-between;

        img {
          width: 310px;
          margin-bottom: 20px;
        }

        #data {
          font-size: 11px;
        }
    }
    .btn-card {
      margin: 50px 0;
      display: flex;
      justify-content: center;
            a {
                background-color: rgb(61, 111, 66);
                color: white;
                text-decoration: none;
                padding: 10px 25px;
                border-radius: 40px;
            }
        }
</style>