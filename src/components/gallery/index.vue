<template>
  <section id="gallery_sec" class=" py-16">
     <v-container>
        <div class="title bg-white d-flex pa-3 mx-auto ga-2 justify-center align-center">
            <span><FeEdit/></span>
            <h6>The Gallery</h6>
        </div>
        <h5  class="pt-5 pb-10">Check Our Recent Work </h5>
        <v-row class="pt-10">
            <v-col v-for="item in gallery" :key="item" cols="3">
                <div class="works">
                    <v-card class="pa-6">
                        <v-img
                        :width="`100%`"
                        aspect-ratio="16/9"
                        cover
                        :src="item['img']"
                        ></v-img>
                        <div class="wrk_info pt-4">
                            <h4 class="pb-1">{{ item['title'] }}</h4>
                            <p>{{ item['subTitle'] }}</p>
                        </div>
                    </v-card>
                </div>
            </v-col>
            <v-col cols="4">
                
            </v-col>
            <v-col cols="4"></v-col>
        </v-row>
     </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import image from '../../assets/gallery/Image.png';
import image2 from '../../assets/gallery/Image2.png';
import image3 from '../../assets/gallery/Image3.png';
import image4 from '../../assets/gallery/Image4.png';
export default {
    name:'GalleryComp',
    components:{FeEdit},
    data(){
        return{
            gallery: [
                {
                    img:image,
                    title:'Electrical & Maintenance',
                    subTitle:'Electric, Instalation',
                },
                {
                    img:image2,
                    title:'Interior/Exterior Services',
                    subTitle:'House, Office',
                },
                {
                    img:image3,
                    title:'Car Repair & Maintenance',
                    subTitle:'Car, Bike, load vehicle',
                },
                {
                    img:image4,
                    title:'Electrical installation',
                    subTitle:'Instalation',
                },
            ]
        }
    }

}
</script>

<style scoped>
    #gallery_sec{
        background: var(--main);
    }
    .title{
        max-width: max-content;
    }
 .title span{
    color: var(--yellow);
    padding-top: 5px;
    display: inline-block;
 }
 .title h6{
    font-family: var(--inter);
    font-weight: 500;
    font-size: 18px;
    color: var(--main);
 }
 h5{
    font-family: var(--mulish);
    font-weight: 900;
    font-size: 45px;
    color: #ffffff;
    text-align: center;
 }
 .works h4{
    font-family: var(--mulish);
    font-weight: 700;
    font-size: 25px;
    color: var(--main);
    text-align: center;
 }
 .works p{
    font-family: var(--inter);
    font-weight: 400;
    font-size: 18px;
    color: var(--sub);
    text-align: center;
 }
</style>