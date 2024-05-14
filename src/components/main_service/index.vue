<template>
  <section id="main_service">
    <v-container>
        <v-row justify="center">
            <v-col cols="8">
                <div class="srvc_box">
                  <div class="title">
                    <h4>Professional Main Services</h4>
                    <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt.</p>
                  </div>
                    <v-card color="transparent mt-10" elevation="0">
                      <v-tabs
                        v-model="tab"
                        align-tabs="center"
                      >
                      <v-tab :value="1" :class="{ 'active_tab mr-10': tab === 1, 'deactive_tab mr-10': tab !== 1 }"> <BsBuildingsFill/> Commercial</v-tab>
                      <v-tab :value="2" :class="{ 'active_tab mr-10': tab === 2, 'deactive_tab mr-10': tab !== 2  }"> <FlFilledDualScreenSettings/> Residential</v-tab>
                      <v-tab :value="3" :class="{ 'active_tab': tab === 3, 'deactive_tab': tab !== 3  }"> <FlFilledBuildingFactory/> Industrial</v-tab>
                      </v-tabs>

                      <v-tabs-window v-model="tab"
                          class="bg-white mt-10 shadow pa-10 elevation-10">
                        <v-tabs-window-item
                          v-for="n in 3"
                          :key="n"
                          :value="n"
                         
                        >
                          <v-container fluid>
                            <v-row>
                             <v-col cols="6">
                              <h6> <span><FlFilledBuilding/></span>
                                Based on Commercial
                              </h6>
                              <h4>Commercial</h4>
                              <p class="pt-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do incididunt ut labore et dolore magna aliqua. Ut enim ad minimquis nostrud exercitation ullamco laboris nisi ut aliquip ex ea 
                              commodo consequat.</p>
                                                            <p>
                              Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.ullamco laboris nisi ut aliquip ex ea 
                              commodo consequat.</p>
                              <div class="read_more">
                                <a href="#">Read More</a>
                              </div>
                             </v-col>
                             <v-col cols="6">
                              <div class="img">
                                <picture>
                                  <img :src="imgOne" :alt="imgOne">
                                </picture>
                              </div>
                             </v-col>
                            </v-row>
                          </v-container>
                        </v-tabs-window-item>
                      </v-tabs-window>
                    </v-card>
                </div>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { BsBuildingsFill } from "@kalimahapps/vue-icons";
import { FlFilledDualScreenSettings } from "@kalimahapps/vue-icons";
import { FlFilledBuildingFactory } from "@kalimahapps/vue-icons";
import { FlFilledBuilding } from "@kalimahapps/vue-icons";
import img from '../../assets/srvc.png'
export default {
    name:'MainService',
    components:{BsBuildingsFill,FlFilledDualScreenSettings,FlFilledBuildingFactory,FlFilledBuilding},
    data () {
      return {
        tab: null,
        imgOne:img,
      }
    },
  
}
</script>

<style scoped>
  #main_service{
    background: var(--yellow);
    padding: 0px 0;
    margin-bottom: 300px;
  }
  .srvc_box{
    position: relative;
    top: 300px;
 
  }
  .shadow{
    box-shadow: 0 5px 10px 0 #bebebe !important;
    margin: 50px;
  }
  .title{
    max-width: 688px;
    margin: 0 auto;
    text-align: center;
  }
  .title h4{
    font-family: var(--mulish);
    font-size: 45px;
    font-weight: 700;
    color: var(--main);
    padding-bottom: 16px;
  }
  .title p{
    font-family: var(--inter);
    font-size: 18px;
    font-weight: 400;
    color: var(--main);
    padding-bottom: 16px;
  }
  h6{
    font-family: var(--inter);
    font-size: 20px;
    font-weight: 500;
    color: var(--main);
    display: flex;
    align-items: center;
    align-content: center;
  }
  h6 span{
    color: var(--yellow);
  }
  h4{
    font-family: var(--mulish);
    font-size: 35px;
    font-weight: 900;
    color: var(--main);
  }
  p{
    font-family: var(--inter);
    font-size: 18px;
    font-weight: 400;
    color: var(--sub);
    padding-bottom: 16px;
  }
  .active_tab{
    font-family: var(--inter);
    font-weight: 400;
    color: var(--main);
    font-size: 24px;
    border-color: #ffffff !important;
    background: #ffffff;

  }
  .deactive_tab{
    font-family: var(--inter);
    font-weight: 400;
    color: var(--main);
    font-size: 24px;
    border: 2px solid var(--main) !important;
    border-color: var(--main) !important;
    background: transparent;
    
  }
  .read_more a{
    font-family: var(--inter);
    font-weight: 600;
    color: var(--main);
    font-size: 20px;
    border: 1px solid var(--yellow) !important;
    background: var(--yellow) !important;
    padding: 20px 40px;
    margin-top: 20px;
    display: inline-block;
  }
  .img img{
    width: 100%;
    height: auto;
    display: block;
  }
</style>