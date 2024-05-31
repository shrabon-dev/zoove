<template>
  <section id="client">
    <v-container>
        <div class="title pb-10">
            <h6> <span><FeEdit/></span> Our Clients</h6>
            <h4>Our Trusted Big Clients!</h4>
        </div>

        <carousel v-bind="settings" :breakpoints="breakpoints">
            <slide v-for="slide in slides" :key="slide">
                <div class="client_img"><picture><img :src="slide.img" :alt="slide.img"></picture></div>
            </slide>
            <!-- <template #addons>
            <navigation />
            <pagination />
            </template> -->
        </carousel>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import img from '../../assets/client/1.svg'
import img2 from '../../assets/client/2.svg'
import img3 from '../../assets/client/3.svg'
import img4 from '../../assets/client/4.svg'
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide } from 'vue3-carousel'
export default {
    name:'OurClient',
    components:{FeEdit, Carousel,
    Slide,},
    data(){
        return{
            img:img,
            img2:img2,
            img3:img3,
            img4:img4,
            slides:[
                {
                    img:img,
                },
                {
                    img:img2,
                },
                {
                    img:img3,
                },
                {
                    img:img,
                },
                {
                    img:img2,
                },
                {
                    img:img4,
                },
                {
                    img:img3,
                },
                {
                    img:img4,
                },
            ],
            settings: {
                itemsToShow: 4,
                snapAlign: 'start',
                },
                // breakpoints are mobile first
                // any settings not specified will fallback to the carousel settings
                breakpoints: {
                // 700px and up
                300: {
                    itemsToShow: 2,
                    snapAlign: 'start',
                },
                // 700px and up
                700: {
                    itemsToShow: 2,
                    snapAlign: 'start',
                },
                // 1024 and up
                1024: {
                    itemsToShow: 4,
                    snapAlign: 'start',
                },
            },
        }
    }

}
</script>

<style scoped>
    .title{
        text-align: center;
        max-width: 600px;
        margin: 0 auto;
    }
    .title h6{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 500;
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

    @media (min-width:300px) and (max-width:600px){
        .title h4{
        font-size: 24px;
        }
        .client_img{
            width: 100%;

        }
        .client_img img{
            width: 80%;
            display: block;
            margin-right: auto;
        }
    }
</style>