<template>
  <footer>
    <v-container>
      <!-- Footer Top Info Start -->
      <v-row>
        <v-col cols="6">
          <div class="logo">
            <picture>
              <img :src="logo" :alt="logo">
            </picture>
          </div>
        </v-col>
        <v-col cols="2">
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
        </v-col>
        <v-col cols="2">
            <div class="d-flex ga-4">
                <div class="icon">
                    <span>
                        <FePhoneCall />
                    </span>
                </div>
                <div class="info">
                    <h6>Call Us</h6>
                    <p class="sml_txt">+880 006854552</p>
                </div>

            </div>
        </v-col>
        <v-col cols="2">
            <div class="d-flex ga-4">
                <div class="icon">
                    <span>
                        <ByLocation />
                    </span>
                </div>
                <div class="info">
                    <h6>Location</h6>
                    <p class="sml_txt">Amsterdam, 109-74</p>
                </div>

            </div>
        </v-col>
       
      </v-row>
      <!-- Footer Top Info End -->
      <!-- Footer Bootom Info Start -->
      <div class="ftr_btm">
        <v-row>
        <v-col cols="5">
         <div class="ftr_dtls">
          <p>Denouncing pleasure and praising pain was born and I will givg you a coghmplete acchount of the system, and expound the actual</p>
           <div class="icons">
            <a href="#"><BsInstagram/></a>
            <a href="#"><AkFacebookFill/></a>
            <a href="#"><BsTwitterX/></a>
            <a href="#"><CoBrandLinkedinIn/></a>
           </div>
         </div>
        </v-col>
        <v-col cols="4">
          <div class="ftr_links">
          <div class="d-flex">
            <div class="link">
            <h5>Explore</h5>
            <ul>
              <li><a href="#">About Us</a></li>
              <li><a href="#">Gallery</a></li>
              <li><a href="#">Offers</a></li>
              <li><a href="#">Pricing</a></li>
              <li><a href="#">FAQ</a></li>
            </ul>
          </div>
          <div class="link">
            <h5>Quick Links</h5>
            <ul>
              <li><a href="#">Services</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact Us</a></li>
              <li><a href="#">Service Request</a></li>
              <li><a href="#">Estimation Calculator</a></li>
            </ul>
          </div>
           </div>
         </div>
        </v-col>
        <v-col cols="3">
          <div class="link">
            <h5>Uitility Pages</h5>
            <ul>
              <li><a href="#">Style Guide</a></li>
              <li><a href="#">Changelog</a></li>
              <li><a href="#">Licenses</a></li>
              <li><a href="#">Protected Page</a></li>
              <li><a href="#">404 Page</a></li>
            </ul>
          </div>
        </v-col>
      </v-row>
      </div>
      <!-- Footer Bootom Info End -->
      <div class="copyright">
        <p>Copyright © BlueCollar | Designed by VictorFlow Templates - Powered by Webflow</p>
      </div>
    </v-container>
  </footer>
</template>

<script>
import flogo from '../../assets/flogo.png'
import { ByMail } from "@kalimahapps/vue-icons";
import { FePhoneCall } from "@kalimahapps/vue-icons";
import { ByLocation } from "@kalimahapps/vue-icons";
import { BsInstagram } from "@kalimahapps/vue-icons";
import { AkFacebookFill } from "@kalimahapps/vue-icons";
import { BsTwitterX } from "@kalimahapps/vue-icons";
import { CoBrandLinkedinIn } from "@kalimahapps/vue-icons";

export default {
    name:'FooterSection',
    components:{ByMail,FePhoneCall,ByLocation,BsInstagram,AkFacebookFill,BsTwitterX,CoBrandLinkedinIn},
    data(){
      return{
        logo:flogo,
      }
    }

}
</script>

<style>
  footer{
    background: var(--main);
    padding: 50px 0;
  }
  .ftr_btm{
    border-bottom: 1px solid #4B557D;
    border-top: 1px solid #4B557D;
    margin: 60px 0;
    padding: 60px 0;
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
    p{
        color: #ffffff;
        font-family:var(--inter) ;
        font-weight: 200;
        font-size: 18px;
    }
    h6{
        font-size: 20px;
        font-weight: 700;
        color: #ffffff;
        font-family: var(--mulish);
    }
    h5{
      font-family: var(--mulish);
      font-weight: 700;
      font-size: 20px;
      color: #e7e7e7;
      padding-bottom: 10px;
    }
    .link{
      padding-left: 100px;
    }
    .ftr_links{
      border-left: 1px solid #4B557D;
      border-right: 1px solid #4B557D;

    }
    ul li a{
      font-family: var(--inter);
      font-weight: 300;
      font-size: 18px;
      color: #e7e7e7;
      padding: 5px 0;
      display: inline-block;
    }
    .icons{
      display: flex;
      gap: 10px;
      align-items: center;
      padding-top: 40px;
    }
    .icons a{
      color: #ffffff;
      width: 50px;
      height: 50px;
      font-size: 20px;
      background: #2C3765;
      border-radius: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: .4s all ease-in;
    }
    .icons a:hover{
      background: var(--yellow);
      color: var(--main);
    }
    .copyright{
      text-align: center;
    }
</style>