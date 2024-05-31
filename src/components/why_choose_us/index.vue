<template>
  <section>
        <v-row align="center" class="gap-10">
            <v-col cols="12" md="6">
                <div class="why_choose_img" :style="bgStyle">
                    <div class="info pa-10">
                        <div class="list">
                            <ul>
                                <li> <span>5263</span> <span> Project Done </span></li>
                                <li> <span>5263</span> <span> People Working</span></li>
                                <li> <span>5263</span> <span> Buisness Partner</span></li>
                                <li> <span>5263</span> <span> Happy Customers</span></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </v-col>
            <v-col cols="12" md="6">
                <div class="why_choose_details pl-4 pl-sm-10">
                    <div class="title">
                        <span><FeEdit/></span>
                        <h6>Why Choose Us </h6>
                    </div>
                    <h4>Few Reasons Why You Should Choose Us</h4>
                    <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt. Interdum et malesuada. </p>
                    <div class="dtls_list">
                        <div class="card_list">
                            <span><AnOutlinedCheck/></span>
                            <div>
                                <h5>35 Years Experiance</h5>
                                <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium </p>
                            </div>
                        </div>
                        <div class="card_list">
                            <span><AnOutlinedCheck/></span>
                            <div>
                                <h5>35 Years Experiance</h5>
                                <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium </p>
                            </div>
                        </div>
                        <div class="card_list">
                            <span><AnOutlinedCheck/></span>
                            <div>
                                <h5>35 Years Experiance</h5>
                                <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium </p>
                            </div>
                        </div>
                        <div class="card_list">
                            <span><AnOutlinedCheck/></span>
                            <div>
                                <h5>35 Years Experiance</h5>
                                <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium </p>
                            </div>
                        </div>
                    </div>
                </div>
            </v-col>
        </v-row>
  </section>
</template>

<script>
import bg from '../../assets/hero.png'
import { FeEdit } from "@kalimahapps/vue-icons";
import { AnOutlinedCheck } from "@kalimahapps/vue-icons";
export default {
    name:'WhyChooseUs',
    components:{FeEdit,AnOutlinedCheck},
    data(){
        return{
            bgStyle:{
                background:`url(${bg})`,
                backgroundSize:'cover',
                backgroundPosition:'center',
                backgroundRepeat:'no-repeate'
            }
        }
    }
}
</script>

<style scoped>
    .why_choose_img{
        padding:140px 0;
    }
    .why_choose_img .info{
        background: #1C275270;        
        backdrop-filter: blur(10px);
        border: 2px solid #1C2752;
        width: max-content;
        margin: 0 auto;
        padding: 180px 115px !important;
    }

    .list ul li {
        position: relative;
        font-family: var(--inter);
        font-size: 24px;
        font-weight: 500;
        color: #ffffff;
        margin-bottom: 10px;
        display: flex;
        align-items: stretch;
  
    }
    .list ul li span:nth-child(1){
        position: relative;
        font-family: var(--inter);
        font-size: 24px;
        font-weight: 700;
        color: var(--main);
        background: var(--yellow);
        display: inline-block;
        width: 80px;
        padding: 10px;
    }
    .list ul li span:nth-child(2){
        border: 2px solid #adadad;
        width: 300px;
        padding: 10px;
    }
    .card_list span{
        width: 20px;
        height: 20px;
        display: inline-block;
        background: var(--yellow);
        color: var(--main);
        border-radius: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .title {
        display: flex;
        align-items: center;
        align-content: center;
        gap:10px;
        padding-bottom: 16px;
    }
    .title span{
        color: var(--yellow);
    }
    .title h6{
        font-family: var(--inter);
        color: var(--main);
        font-size: 18px;
        font-weight: 500;
    }
    h4{
        font-family: var(--mulish);
        color: var(--main);
        font-size: 45px;
        font-weight: 900;
        max-width: 60%;
        line-height: 1.3;
        padding-bottom: 16px;
    }
    p{
        font-family: var(--inter);
        color: var(--sub);
        font-size: 18px;
        font-weight: 400;
        max-width: 60%;
        line-height: 1.7;
        padding-bottom: 20px;
    }
    h5{
        font-family: var(--mulish);
        color: var(--main);
        font-size: 20px;
        font-weight: 700;
        margin-bottom: 0;
        padding-bottom: 0;
    }
    .card_list{
        display: flex;
        gap: 10px;
        align-items: start;
        align-content: start;
    }
    @media (min-width:300px) and (max-width:600px) {
        .why_choose_img{
            padding: 50px 0;
        }
        .why_choose_img .info{
            padding: 20px !important;
        }
        .list ul li{
            font-size: 16px;
        }
        .list ul li span:nth-child(1){
        font-size: 14px;
        width: 60px;
        }
        .list ul li span:nth-child(2){
            width: 200px;
        }
        h4{
            font-size: 32px;
            max-width: 90%;
        }
        p{
            font-size: 14px;
            max-width: 90%;
        }
        .card_list span{
            width: 24px !important;
            height: 24px !important;
            font-size: 20px;
            padding: 2px;
        }
    }
    @media (min-width:601px) and (max-width:960px) {
        h4{
            max-width: 90%;
        }
        p{
            max-width: 90%;
        }
    }
    @media (min-width:961px) and (max-width:1280px) {
        h4{
            max-width: 90%;
        }
        p{
            max-width: 90%;
        }
        .why_choose_img{
            padding: 160px 0;
        }
        .why_choose_img .info{
            padding: 100px 50px !important;
        }
    }
</style>