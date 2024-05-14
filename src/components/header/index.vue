<template>
  <header class="">
    <v-container>
        <div class="hdr_top">
            <v-row justify="justify-space-between">
                <v-col cols="6">
                    <p>Opening Hours: 06:00 to 20:00</p>
                </v-col>
                <v-col cols="6" class="text-right">
                    <ul class="d-flex justify-end ga-10">
                        <li><a href="#"><AkInstagramFill/></a></li>
                        <li><a href="#"><FaBandsFacebookF/></a></li>
                        <li><a href="#"><BsTwitterX/></a></li>
                        <li><a href="#"><CoBrandLinkedinIn/></a></li>
                    </ul>
                </v-col>
            </v-row>
        </div>
        <div class="hdr_btm pt-10">
            <v-row justify="between">
                <v-col>
                    <!-- Logo Start -->
                    <div class="logo">
                        <picture>
                            <img class="" :src="logo" :alt="logo">
                        </picture>
                    </div>
                </v-col>
                <v-col>
                    <!-- Icons Start -->
                    <div class="d-flex justify-end ga-10">
                        <div class="w-1/2">
                            <div class="d-flex ga-4">
                                <div class="icon">
                                    <span>
                                        <ByMail />
                                    </span>
                                </div>
                                <div class="info">
                                    <h6>Mail Us</h6>
                                    <p class="sml_txt">info@example.com</p>
                                </div>

                            </div>
                        </div>
                        <div class="w-1/2">
                            <div class="d-flex ga-4">
                                <div class="icon">
                                    <span>
                                        <FePhoneCall />
                                    </span>
                                </div>
                                <div class="info">
                                    <h6>Call Us</h6>
                                    <p class="sml_txt">+880 0011262565</p>
                                </div>

                            </div>
                        </div>
                    </div>

                </v-col>
            </v-row>
        </div>
    </v-container>
  </header>
</template>

<script>
import { AkInstagramFill } from "@kalimahapps/vue-icons";
import { FaBandsFacebookF } from "@kalimahapps/vue-icons";
import { BsTwitterX } from "@kalimahapps/vue-icons";
import { CoBrandLinkedinIn } from "@kalimahapps/vue-icons";
import logo from '../../assets/logo.png'
import { ByMail } from "@kalimahapps/vue-icons";
import { FePhoneCall } from "@kalimahapps/vue-icons";
export default {
    name:'HeaderSection',
    components:{
        AkInstagramFill,FaBandsFacebookF,BsTwitterX,CoBrandLinkedinIn,ByMail,FePhoneCall
    },
    data(){
        return{
            logo:logo,
        }
    }
}
</script>

<style scoped>
    p{
        color: var(--main);
        font-family:var(--inter) ;
        font-weight: 400;
        font-size: 18px;
    }
    .sml_txt{
        color: #7E7E7E;
    }
    a{
        color: var(--main);
        font-size: 18px;
    }
    .logo img{
        width: 200px;
    }
    .icon span{
        font-size: 32px;
        background: var(--yellow);
        width:60px;
        height:60px;
        display: inline-flex;
        justify-content: center;
        align-items: center;
        border:1px solid var(--yellow);
        border-radius: 100%;
        color: var(--main);
    }
    h6{
        font-size: 20px;
        font-weight: 700;
        color: var(--main);
        font-family: var(--mulish);
    }


</style>