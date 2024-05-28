<template>
  <section id="future_sec">
    <v-container>
        <v-row justify="center">
            <v-col cols="12" sm="6" md="5" lg="4">
                <div class="ftr_img">
                    <picture>
                        <img :src="img" :alt="img">
                    </picture>
                </div>
            </v-col>
            <v-col cols="12" sm="6" md="7" lg="4">
                <div class="ftr_detls">
                    <h6>
                        <img :src="slogo" :alt="slogo"> Welcome Zoova
                    </h6>
                    <h4>We Provide Your Future</h4>
                    <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt.</p>
                    <p> Interdum et malesuada. In pulvinar viverra diam, nec rutrum mauris maximus non. Aenean sed quam tristique, facilisis est ac, interdum velit.</p>

                    <div class="d-flex align-center align-sm-center align-lg-end">
                        <div class="exp">
                            <span>35</span>
                            <h3>Years Of Experiance</h3>
                        </div>
                        <div class="exp_list ">
                            <ul>
                                <li> - Sed varius ipsum lacus</li>
                                <li> - Pulvinar tortor dignissim sit amet.</li>
                                <li> - Quisque tristique diam quis placerat</li>
                                <li> - Aliquam id ante suscipi fringilla.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import imgOne from '../../assets/future.jpg' 
import slogo from '../../assets/slogo.svg' 

export default {
    name:'FutureComp',
    components:{},
    data(){
        return{
            img:imgOne,
            slogo:slogo,
        }
    }
}
</script>

<style scoped>
    #future_sec{
        padding: 100px 0;
    }
    .ftr_img {
        text-align: right;
        width: 100%;
    }
    .ftr_img img{
        width: 100%;
        display: block;
        margin-left: auto;
    }

    h6{
        font-size: 20px;
        color: var(--main);
        font-family: var(--inter);
        font-weight: 500;
        display: flex;
        justify-items: center;
        align-items: center;
        margin-top: 20px;
    }
    p{
        font-size: 18px;
        color: var(--sub);
        font-family: var(--inter);
        font-weight: 300;
        max-width: 600px;
        padding-bottom: 20px;
        line-height: 1.3;
    }
    .exp_list{
        padding-top: 20px;
    }
    ul li{
        font-size: 18px;
        color: var(--sub);
        font-family: var(--inter);
        font-weight: 300;
        padding-bottom: 10px;
        line-height: 1.3;
    }
    h4{
        font-size: 45px;
        color: var(--main);
        font-family: var(--mulish);
        font-weight: 900;
        margin-bottom: 20px;

    }
    .exp{
        text-align: center;
        padding-left: 60px;
        padding-right: 60px;
        padding-top: 0;
    }
    .exp span{
        font-size: 66px;
        color: var(--yellow);
        font-family: var(--mulish);
        font-weight: 900;
    }
    .exp h3{
        font-size: 24px;
        color: var(--main);
        font-family: var(--mulish);
        font-weight: 900;
        line-height: 1;
        max-width: 110px;
    }
    @media (min-width:300px) and (max-width:600px) {
        .exp{
            padding: 0 20px;
            padding-left: 0px;
        }
        .exp h3{
            font-size: 16px;
        }
        .exp span{
            font-size: 40px;
        }
        ul li{
            font-size: 12px;
        }
        p{
            font-size: 16px;
        }
        h4{
            font-size: 28px;
            padding-top: 8px;
            line-height: 1.3;
        }
        h6{
            font-size: 16px;
        }
    }
</style>