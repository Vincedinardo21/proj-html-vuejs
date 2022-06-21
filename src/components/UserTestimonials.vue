<template>
    <!-- Up -->
    <section>    
            <div class="container">
                <div class="row">
                    <div class="col-12 height">
                        <h2>Users Testimonials</h2>
                        <div class="card-container">
                            <div class="my-card" v-for="(item, i) in testimonials" :key="i">
                                <img :src="item.image" :alt="item.user">
                                <p>{{item.text}}</p>
                                <div>{{item.user}}</div>
                            </div>
                        </div>                
                    </div>
                </div>
            </div>   
    </section>    
</template>

<script>
export default {
  name: 'UserTestimonials',  
  data(){
    return {
        testimonials : [
            {
                image : require("../assets/img/avatar-3.jpg"),
                text : "Auctor est abitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, trincidunt eu. Eu.",
                user : "Lisa Smith, ThemeFusion"
            },
            {
                image : require("../assets/img/avatar-1.jpg"),
                text : "Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget felicis porttitor volutpat vestibulum ac diam sit.",
                user : "Melissa Green, ThemeFusion"
            },
            {
                image : require("../assets/img/avatar-4.jpg"),
                text : "Curubitur arcu erat, accumsan id imperdiet et, porttitor at sem. Proin eget tortor risus vestibulum ante ipsum.",
                user : "Sam Lewis, ThemeFusion"
            }
        ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    section {
        
        text-align: center;
        color: white;
        background-image: url("../assets/img/bg-transparent-3.png");
        background-color: #2a382a;
        background-repeat: repeat-x;
        

        .height {
            height: 550px;
        }
    }
   .card-container {
        display: flex;
        justify-content: space-between;

        img {
            width: 100px;
            border-radius: 50px;
        }
   }
</style>