<template>
  <section id="price_plan">
    <v-container>
        <v-row>
            <v-col cols="12" sm="12" md="12" lg="8" xl="8" class="mx-auto">
                <div class="title">
                    <h6> <span><FeEdit/></span> Price and Plan</h6>
                    <div class="d-sm-flex">

                        <h4 class="w-sm-50">Let’s Customize Work With Affordable Price</h4>
                        <p class="w-sm-50">Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt. Interdum et malesuada.</p>
                    </div>
                </div>
                <v-row justify="center">
                    <v-col cols="12" sm="6" md="4">
                        <div class="plan pa-lg-1 pa-xl-8">
                            <div class="price d-flex justify-between align-center">
                                <div class="w-50">
                                    <span>Basic Plan</span>
                                    <h2>$599.00</h2>
                                </div>
                                <div class="w-50">
                                    <h6>Per Visit Charge</h6>
                                </div>
                            </div>
                            <div class="plan_info">
                                <ul>
                                    <li><span><AkCircleCheck/></span> Electrical Service</li>
                                    <li><span><AkCircleCheck/></span> Distribution Power Systemss</li>
                                    <li><span><AkCircleCheck/></span> High & Medium Voltages</li>
                                    <li><span><AkCircleCheck/></span> Industrial Control Systems</li>
                                    <li><span><AkCircleCheck/></span> Switch Installation</li>
                                    <li><span><AkCircleCheck/></span> Generator Installations</li>
                                    <li><span><AkCircleCheck/></span> Innovative Construction</li>
                                </ul>

                                <!-- Button Start -->
                                <button>Buy Now</button>
                                <!-- Button End -->
                            </div>
                        </div>
                    </v-col>
                    <v-col cols="12" sm="6" md="4">
                           <div class="plan standard pa-lg-1 pa-xl-8">
                            <div class="price d-flex justify-between align-center">
                                <div class="w-50">
                                    <span>Standard</span>
                                    <h2>$999.00</h2>
                                </div>
                                <div class="w-50">
                                    <h6>Per Visit Charge</h6>
                                </div>
                            </div>
                            <div class="plan_info">
                                <ul>
                                    <li><span><AkCircleCheck/></span> Electrical Service</li>
                                    <li><span><AkCircleCheck/></span> Distribution Power Systemss</li>
                                    <li><span><AkCircleCheck/></span> High & Medium Voltages</li>
                                    <li><span><AkCircleCheck/></span> Industrial Control Systems</li>
                                    <li><span><AkCircleCheck/></span> Switch Installation</li>
                                    <li><span><AkCircleCheck/></span> Generator Installations</li>
                                    <li><span><AkCircleCheck/></span> Innovative Construction</li>
                                </ul>

                                <!-- Button Start -->
                                <button>Buy Now</button>
                                <!-- Button End -->
                            </div>
                        </div>
                    </v-col>
                    <v-col cols="12" sm="6" md="4">
                           <div class="plan pa-lg-1 pa-xl-8">
                            <div class="price d-flex justify-between align-center">
                                <div class="w-50">
                                    <span>Professional</span>
                                    <h2>$1299.00</h2>
                                </div>
                                <div class="w-50">
                                    <h6>Per Visit Charge</h6>
                                </div>
                            </div>
                            <div class="plan_info">
                                <ul>
                                    <li><span><AkCircleCheck/></span> Electrical Service</li>
                                    <li><span><AkCircleCheck/></span> Distribution Power Systemss</li>
                                    <li><span><AkCircleCheck/></span> High & Medium Voltages</li>
                                    <li><span><AkCircleCheck/></span> Industrial Control Systems</li>
                                    <li><span><AkCircleCheck/></span> Switch Installation</li>
                                    <li><span><AkCircleCheck/></span> Generator Installations</li>
                                    <li><span><AkCircleCheck/></span> Innovative Construction</li>
                                </ul>

                                <!-- Button Start -->
                                <button>Buy Now</button>
                                <!-- Button End -->
                            </div>
                        </div>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import { AkCircleCheck } from "@kalimahapps/vue-icons";
export default {
    name:'PricePlan',
    components:{FeEdit,AkCircleCheck}
}
</script>

<style scoped>
#price_plan{
    padding: 100px 0;
}
   .title{
        margin: 0 auto;
    }
    .title h6{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);
        display: flex;
        align-items: center;
        align-content: center;
        justify-content: left;
        gap: 10px;
    }
    .title h6 span{
        color: var(--yellow);
    }
    .title h4{
        font-family: var(--mulish);
        font-size: 45px;
        font-weight: 900;
        color: var(--main);
    }
    .title p{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--sub);
    }
    .price {
        border-bottom: 1px solid #7E7E7E;
        padding: 10px 0;
        margin-bottom: 20px;
    }
    .price span{
        font-family: var(--inter);
        font-weight: 700;
        font-size: 20px;
        color: var(--main);
    }
    .price h2{
        font-family: var(--mulish);
        font-weight: 900;
        font-size: 32px;
        color: var(--main);
    }
    .price h6{
        font-family: var(--inter);
        font-weight: 400;
        font-size: 16px;
        color: #7E7E7E;
    }
    .plan_info li{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: #7E7E7E;
        display: flex;
        align-items: center;
        align-content: center;
        gap: 10px;
    }
    .plan_info li span {
        color: var(--yellow);
        padding-right: 10px;
        display: inline;
        margin-top: 4px;
        padding: 0;
    }
    .plan button{
        background: var(--yellow);
        padding: 10px 0;
        width: 100%;
        font-family: var(--inter);
        font-size: 20px;
        font-weight: 600;
        color: var(--main);
        border: 2px solid var(--yellow);
        margin-top: 60px;
        position: relative;
        overflow: hidden;
        transition: .4s all ease-in-out;
    }
    .standard button{
        background: transparent;
        color: var(--yellow);
    }
    button::after{
    position: absolute;
    top: 0%;
    left: -100%;
    background: transparent;
    box-shadow: 0 0 20px 0 #000000;
    width: 50px;
    height: 50px;
    content: '';
    transform: rotate(45deg) translate(-50%,50%);
    transition: .4s all ease-in-out;
  }
  button:hover{
    background: #000000 !important;
    color: #ffffff;
  }
  button:hover:after{
    background: var(--yellow);
    left: -2%;
  }
    @media (min-width:300px) and (max-width:600px){
        .title h6{
            font-size: 18px;
        }
        .title h4{
            font-size: 24px;
            padding-bottom: 10px;
        }
        .title p{
            font-size: 14px;
        }
    }
    @media (min-width:1280px) and (max-width:1499px){
        .title h6{
            font-size: 18px;
        }
        .title h4{
            font-size: 24px;
            padding-bottom: 10px;
        }
        .title p{
            font-size: 14px;
        }
        .plan_info li{
            font-size: 14px;
        }
        .price h2{
            font-size: 24px;
        }
        .price span{
            font-size: 16px;
        }
        .price h6{
            font-size: 14px;
        }
    }
</style>