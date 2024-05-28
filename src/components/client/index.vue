<template>
  <section id="client">
    <v-container>
        <div class="title pb-10">
            <h6> <span><FeEdit/></span> Our Clients</h6>
            <h4>Our Trusted Big Clients!</h4>
        </div>
        <v-row justify="center" class="pt-10">
            <v-col cols="2"><div class="client_img"><picture><img :src="img" :alt="img"></picture></div></v-col>
            <v-col cols="2"><div class="client_img"><picture><img :src="img2" :alt="img2"></picture></div></v-col>
            <v-col cols="2"><div class="client_img"><picture><img :src="img3" :alt="img3"></picture></div></v-col>
            <v-col cols="2"><div class="client_img"><picture><img :src="img4" :alt="img4"></picture></div></v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import img from '../../assets/client/1.svg'
import img2 from '../../assets/client/2.svg'
import img3 from '../../assets/client/3.svg'
import img4 from '../../assets/client/4.svg'
export default {
    name:'OurClient',
    components:{FeEdit},
    data(){
        return{
            img:img,
            img2:img2,
            img3:img3,
            img4:img4,
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
</style>