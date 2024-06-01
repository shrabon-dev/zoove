<template>
  <nav :class="[menu ?'mble-menu-active':'mble-menu-deactive']">
    <v-container class="bg pa-0">
          <div  class="d-sm-flex pa-0 justify-space-between align-center">
            <v-col cols="12" sm="9" md="9" lg="9" xl="10" class="">
              <!-- Menu Bar Start -->
              <ul class="d-sm-flex justify-end ga-10">
                <li><a href="#">Home</a></li>
                <li><a href="#">About us</a></li>
                <li><a href="#">Pages</a></li>
                <li><a href="#">Our Services</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact us</a></li>
              </ul>
              <!-- Menu Bar End -->
            </v-col>
            <v-col cols="12" sm="3" md="3" lg="3" xl="2" class="text-md-right ">
              <!-- Button Start -->
              <a class="btn" href="#">Have Any Questions?</a>
              <!-- Button End -->
            </v-col>
          </div>
         
    </v-container>
  </nav>
</template>

<script>
import  EventBus  from '../../eventBus';
export default {
    name:'NavBar',
    data() {
    return {
      menu: ''
    };
    },
    mounted() {
        EventBus.on('messageSent', this.updateMessage);
    },
    beforeUnmount() {
        EventBus.off('messageSent', this.updateMessage);
    },
    methods: {
        updateMessage(msg) {
            this.menu = msg;
        }
    }
}
</script>

<style scoped>
  nav{
   position: relative;
   bottom: -55px; 
   z-index: 999999;
  }
  nav .bg{
    background: var(--yellow);
  }
  ul li a{
    color:var(--main);
    font-family:var(--inter);
    font-size: 20px;
    font-weight: 700;
  }
  .btn{
    display: inline-block;
    color:#ffffff;
    font-family:var(--inter);
    font-size: 20px;
    font-weight: 500;
    background: var(--main) !important;
    padding: 20px 20px;
    transition: .4s all ease-in-out;
    overflow: hidden;
    position: relative;
  }
  .btn::after{
    position: absolute;
    top: 15%;
    left: -100%;
    background: transparent;
    box-shadow: 0 0 20px 0 #000000;
    width: 50px;
    height: 50px;
    content: '';
    transform: rotate(45deg) translate(-50%,50%);
    transition: .4s all ease-in-out;
  }
  .btn:hover{
    background: #000000 !important;
  }
  .btn:hover:after{
    background: var(--yellow);
    left: -2%;
  }
  @media (min-width:300px) and (max-width:600px) {
    ul li a{
      font-size: 14px;
      padding-bottom: 12px;
    }
    .btn{
      font-size: 14px;
      padding: 10px 20px;
    }
    .mble-menu-deactive {
    height: 0;
    overflow: hidden;
    transition: height 0.4s ease-in-out;
    opacity: 0;
  }
  .mble-menu-active {
    position: absolute;
    width: 100%;
    z-index: 99999;
    left: 0;
    top: 100px;
    height: auto;
    opacity: 1;
    transition: height 0.4s ease-in-out;
  }
  }
  @media (min-width:601px) and (max-width:960px) {
    ul li a{
      font-size: 14px;
    }
    .btn{
      font-size: 14px;
      padding: 10px 10px;
    }
    
  }
  @media (min-width:961px) and (max-width:1279px) {
    nav{
      bottom: -30px;
    }
    ul li a{
      font-size: 14px;
    }
    .btn{
      font-size: 14px;
      padding: 10px 10px;
    }
    
  }
</style>