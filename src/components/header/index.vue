<template>
    <header class="">
        <v-container>
            <div class="hdr_top">
                <v-row justify="justify-space-between" align="center">
                    <v-col cols="6">
                        <p class="">Opening Hours: <span>06:00 to 20:00</span></p>
                    </v-col>
                    <v-col cols="6" class="text-right">
                        <ul class="d-flex justify-end ga-sm-10 ga-3">
                            <li><a href="#">
                                    <AkInstagramFill />
                                </a></li>
                            <li><a href="#">
                                    <FaBandsFacebookF />
                                </a></li>
                            <li><a href="#">
                                    <BsTwitterX />
                                </a></li>
                            <li><a href="#">
                                    <CoBrandLinkedinIn />
                                </a></li>
                        </ul>
                    </v-col>
                </v-row>
            </div>
            <div class="hdr_btm pt-5">
                <v-row justify="between">
                    <v-col sm="4" md="4" lg="5" order="1" order-sm="1">
                        <!-- Logo Start -->
                        <div class="logo">
                            <picture>
                                <img  class="" :src="logo" :alt="logo">
                            </picture>
                        </div>
                    </v-col>
                    <v-col order="2" class="d-block d-sm-none" >
                        <div class="menu text-right">
                            <span @click="sendMessage"><AnOutlinedMenu/></span>
                        </div>
                    </v-col>
                    <v-col sm="8" md="8" lg="7" order="1" order-sm="2" class="d-none d-sm-block ">
                        <!-- Icons Start -->
                        <div class="d-flex justify-end ga-2 ga-sm-3 ga-md-10">
                            <div class="w-50 w-lg-33 w-xl-33">
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
                            <div class="w-50 w-lg-50 w-xl-33">
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
import { AnOutlinedMenu } from "@kalimahapps/vue-icons";
import  EventBus  from  '../../eventBus';
export default {
    name: 'HeaderSection',
    components: {
        AkInstagramFill, FaBandsFacebookF, BsTwitterX, CoBrandLinkedinIn, ByMail, FePhoneCall,AnOutlinedMenu
    },
    data() {
        return {
            logo: logo,
            menu:false,
        }
    },
    methods: {
    sendMessage() {
      this.menu = !this.menu
      EventBus.emit('messageSent', this.menu);
    }
    },
}
</script>

<style scoped>
p {
    color: var(--main);
    font-family: var(--inter);
    font-weight: 400;
    font-size: 18px;
}

.sml_txt {
    color: #7E7E7E;
}

a {
    color: var(--main);
    font-size: 18px;
}

.logo img {
    width: 200px;
}

.icon span {
    font-size: 32px;
    background: var(--yellow);
    width: 60px;
    height: 60px;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    border: 1px solid var(--yellow);
    border-radius: 100%;
    color: var(--main);
}

h6 {
    font-size: 20px;
    font-weight: 700;
    color: var(--main);
    font-family: var(--mulish);
}

@media (min-width:300px) and (max-width:600px) {
    p {
        font-size: 10px;
    }
    p span{
        display: block;
    }

   

    a {
        font-size: 14px;
    }

    h6 {
        font-size: 14px;
    }

    .icon span {
        width: 30px;
        height: 30px;
        font-size: 14px;
    }

    .info p {
        font-size: 10px;
    }
    .logo img {
        width: 100px;
    }
}
</style>