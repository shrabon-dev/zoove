<template>
  <section id="service_sec">
    <v-container>
        <div class="title">
            <h6> <span><FeEdit/></span> Our Service</h6>
            <h4>Our Services</h4>
            <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt.</p>
        </div>
        <v-row justify="center" class="pt-10">
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
                        <McAirConditionOpenLine/>
                    </div>
                    <h5>Air condition service </h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
                        <MdSharpElectricMeter/>
                    </div>
                    <h5>Electrical installation</h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
                        <BsBuildingsFill/>
                    </div>
                    <h5>General Builder</h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
                        <BsBuildingFillLock/>
                    </div>
                    <h5>Security System</h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
            
                        <MdSharpDesignServices/>
                    </div>
                    <h5>Service & maintenance</h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="4" lg="4" xl="3">
                <div class="srvce_card pa-5 pa-sm-5 pa-md-5 pa-lg-10">
                    <div class="srvce_img">
                        <!-- <picture>
                            <img :src="air" :alt="air">
                        </picture> -->
                        <BsHouseCheck/>
                    </div>
                    <h5>House Extensions</h5>
                    <p>Sagittis Nulla facilisi. In sed pretium metus. Proin pretium Turna sit amet tincidunt.</p>
                    <a href="#">Read More...</a>
                </div>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import air from '../../assets/service/air.png'
import { McAirConditionOpenLine } from "@kalimahapps/vue-icons";
import { MdSharpElectricMeter } from "@kalimahapps/vue-icons";
import { BsBuildingsFill } from "@kalimahapps/vue-icons";
import { BsBuildingFillLock } from "@kalimahapps/vue-icons";
import { MdSharpDesignServices } from "@kalimahapps/vue-icons";
import { BsHouseCheck } from "@kalimahapps/vue-icons";
export default {
    name:'ServiceComp',
    components:{FeEdit,McAirConditionOpenLine,MdSharpElectricMeter,BsBuildingsFill,BsBuildingFillLock,MdSharpDesignServices,BsHouseCheck},
    data(){
        return{
            air:air,
        }
    }

}
</script>

<style scoped>
    #service_sec{
        padding-bottom: 100px;
    }
    .title{
        text-align: center;
        max-width: 600px;
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
        justify-content: center;
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
        padding-top: 10px;
    }
    .srvce_card{
        background: var(--main);
    }
    .srvce_card h5{
        font-family: var(--mulish);
        font-size: 25px;
        font-weight: 500;
        color: var(--yellow);
    }
    .srvce_card p{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 300;
        color: #D2D2D2;

    }
    .srvce_card a{
        display: inline-block;
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 500;
        color: #ffffff;
        padding-top: 30px;
    }
    .srvce_img {
        font-size: 74px;
        color: var(--yellow);
    }
    @media (min-width:300px) and (max-width:600px) {
    
    .title h6{
        font-family: var(--inter);
        font-size: 16px;
        font-weight: 400;
        color: var(--main);
        display: flex;
        align-items: center;
        align-content: center;
        justify-content: center;
        gap: 10px;
    }
    .title h4{
        font-size: 32px;
    }
    .title p{
        font-size: 16px;
    }
    }
    @media (min-width:960px) and (max-width:1280px) {
     .srvce_card{
        max-height: 400px;
        min-height: 300px;
     }
     .srvce_card h5{
        font-size: 20px;
     }
     .srvce_card p{
        font-size: 16px;
     }
     .srvce_card a{
        font-size: 16px;
     }
    }
</style>