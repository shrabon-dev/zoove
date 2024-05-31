<template>
    <Carousel :autoplay="2000" v-bind="settings">
        <Slide v-for="slide in 10" :key="slide">
  <section id="hero" :style="bgStyle">
   <div class="overlay">
    <v-container>
      <!-- <v-row>
        <v-col cols="12" sm="10" md="7">
          <h6> <span><GlSettings/></span> We Provide Electric Services For Industrial Project</h6>
          <h2>We Are Professional Quality Services</h2>
          <div class="btn">
            <a href="#">Our Services</a>
          </div>
        </v-col>

      </v-row> -->
    
          <div class="hr_info text-left">
            <h6> <span><GlSettings/></span> We Provide Electric Services For Industrial Project</h6>
            <h2>We Are Professional Quality Services</h2>
            <div class="btn">
              <a href="#">Our Services</a>
            </div>
          </div>
   
    </v-container>
   </div>
  </section>
</Slide>

       
</Carousel>
</template>

<script>
import banner from '../../assets/hero.png'
import { GlSettings } from "@kalimahapps/vue-icons";
import { Carousel, Slide } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'
export default {
    name:'HeroSection',
    components:{GlSettings,Carousel,
    Slide,},
    data(){
      return{
        bgStyle:{
          background:`url(${banner})`,
          backgroundSize:'cover',
          backgroundPosition:'center',
          backgroundRepeat:'no-repeat',
          width:'100%',
        },
        settings: {
          itemsToShow: 1,
          snapAlign: 'start',
        },
      }
    }
}
</script>

<style scoped>
  .overlay{
    background: radial-gradient(circle,#000000 0%,#00000000 0%,#000000 70%);
    padding: 200px 0;
  }
  h6{
    font-family: var(--inter);
    font-size: 18px;
    font-weight: 500;
    background: #ffffff50;
    padding: 5px 10px;
    display: inline-flex;
    align-items: center;
    align-content: center;
    color: #ffffff;
    
  }
  h6 span{
    color: var(--yellow);
    padding-right: 10px;
    padding-top: 2px;
  }
  h2{
    font-family: var(--mulish);
    font-size: 60px;
    font-weight: 900;
    line-height: 1.3;
    color: #ffffff;
    margin-top: 24px;
    max-width: 700px;
    
  }

  .btn a{
    display: inline-block;
    background: var(--yellow);
    padding: 10px 20px;
    font-family: var(--inter);
    font-size: 20px;
    font-weight: 500;
    color: var(--main);
    margin-top: 34px;

  }
  @media (min-width:300px) and (max-width:600px){
  .overlay{
    padding: 60px 0;
  }
  h2{
  font-size: 30px;
  }
}
</style>