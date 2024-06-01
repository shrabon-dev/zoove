<template>
  <section id="testimonial">
    <v-container>
        <v-row justify="center">
             <v-col cols="12" sm="6" md="6" lg="4">
                <!-- Title Start -->
                <div class="title">
                    <span>
                        <FeEdit/>
                    </span>
                    <h6>Testmonial</h6>
                </div>
                <!-- Title End -->
                <!-- Feedback Start -->
                <v-card class="pb-5 pl-5">
                    <!-- Slider Message Start -->
                     <div class="feedback">
                        <div class="fdr_hdr d-flex justify-start align-center ga-5 border-b pb-2 position-relative">
                            <div class="img rounded-circle">
                                <picture>
                                    <img class="rounded-circle" src="https://miro.medium.com/v2/resize:fit:850/1*nq9cdMxtdhQ0ZGL8OuSCUQ.jpeg" alt="">
                                </picture>
                            </div>
                            <div class="hdr_info">
                                <h4>Muhammad Ali</h4>
                                <h6>Bangladesh</h6>
                            </div>
                            <span class="qoute">
                                <CaQuotes/>
                            </span>
                        </div>
                        <div class="fdbk">
                            <p class="py-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, necessitatibus. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Suscipit nulla similique neque sint ex, impedit voluptatem optio corrupti velit iure!</p>
                        </div>
                        <div class="icon">
                            <span class="lft"><BsChevronLeft/></span>
                            <span class="rgt"><BsChevronRight/></span>
                        </div>
                     </div>
                    <!-- Slider Message End -->
                </v-card>
                <!-- Feedback End -->
                <!-- Any Question Start -->
                <div class="any_question">
                    <v-card class="card_bg">
                        <div class="title bg-white pa-1 d-inline-flex ga-0 pr-4 mb-4">
                            <span>
                                <FeEdit/>
                            </span>
                            <h6>Any Question</h6>
                        </div>
                        <h4>99.9% Customer Satisfation Based</h4>
                        <p>If you have any questions or need help contact with our team, or call</p>
                        <div class="d-flex align-center">
                            <span><FlCall/></span>
                            <h5>(003) 123 456 7890</h5>
                        </div>
                    </v-card>
                </div>
                <!-- Any Question End -->
             </v-col>
             <v-col cols="12" sm="6" md="6" lg="4">
                <!-- Title Start -->
                <div class="title pb-0 mb-0">
                    <span>
                        <FeEdit/>
                    </span>
                    <h6>Meet us</h6>
                </div>
                <!-- Title End -->
                <!-- Feedback Start -->
                    <h3>Appointment Form</h3>
                   <!-- Form Input -->
                   <div class="form pt-5  pa-md-10">
                    <form action="" method="post">
                      <input type="text" placeholder="Your Name">
                      <input type="text" placeholder="Email Address">
                      <input type="text" placeholder="Phone Number">
                      <input type="text" placeholder="Date">
                      <textarea name="" id="" cols="30" rows="10" placeholder="Service Description"></textarea>
                      <button class="bg  btn" :height="60"  :width='`100%`'>Submit</button>
                   </form>
                   </div>

                <!-- Feedback End --> 
             </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import { BsChevronLeft } from "@kalimahapps/vue-icons";
import { BsChevronRight } from "@kalimahapps/vue-icons";
import { CaQuotes } from "@kalimahapps/vue-icons";
import { FlCall } from "@kalimahapps/vue-icons";
export default {
    name:'TestimonialComp',
    components:{FeEdit,BsChevronLeft,BsChevronRight,CaQuotes,FlCall}
}
</script>

<style scoped>
  .title{
        margin: 0 auto;
        display: flex;
        align-items: center;
        align-content: center;
        padding: 30px 0;
        gap: 10px;
    }
    .bg{
        background: var(--yellow);
        color: var(--main);
        font-family: var(--inter);
    }
    input,textarea{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--sub);
        width: 100%;
        display: block;
        border: 1px solid #dbdbdb;
        border-radius: 2px;
        margin-bottom: 10px;
        padding: 6px;
    }
    textarea{
        height: 202px;
        resize: none;
    }
    ::placeholder{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--sub);
    }
    button{
        font-family: var(--inter);
        font-size: 20px;
        font-weight: 700;
        color: var(--main);
    }
    .title h6{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);

    }

    .feedback .img{
        width: 60px;
        height: 60px;
    }
    .feedback .img img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        image-resolution:initial;
        image-rendering: pixelated;
        display: block;
    }
    .icon{
        display: flex;
        align-items: center;
        gap: 10px;
        color:var(--main)
    }
    .icon span{
        width: 40px;
        height: 40px;
        background: transparent;
        border: none;
        border-radius: 100%;
        font-size: 18px;
        line-height: 40px;
        text-align: center;
        transition: .4s all ease-in-out;
        cursor: pointer;
    }
    .icon span:hover{
        background:  var(--yellow);
    }

    .qoute{
        font-size: 24px;
        width: 40px;
        height: 40px;
        border-radius: 100%;
        background:  var(--yellow);
        color: var(--main);
        text-align: center;
        line-height: 40px;
        position: absolute;
        top: 10px;
        right: 60px;
    }
    .hdr_info h4{
        font-family: var(--mulish);
        font-size: 20px;
        font-weight: 700;
        color: var(--main);
    }
    h3{
        font-family: var(--mulish);
        font-size: 35px;
        font-weight: 900;
        color: var(--main);
    }
    .hdr_info h6{
        font-family: var(--inter);
        font-size: 14px;
        font-weight: 400;
        color: var(--sub);
    }
    .fdbk p{
        font-family: var(--inter);
        font-size: 16px;
        font-weight: 400;
        color: var(--sub);
        max-width: 500px;
        font-style: italic;
    }
    .any_question .card_bg{
        background: var(--yellow);
        color: var(--main);
        width: 100%;
        padding: 20px;
    }
    .any_question h4{
        font-family: var(--mulish);
        font-size: 24px;
        font-weight: 900;
    }
    .any_question p{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);
        padding: 12px 0 20px 0;
    }
    .any_question h5{
        font-family: var(--mulish);
        font-size: 24px;
        font-weight: 900;
        margin-left: 10px;

    }
    .any_question span{
        width: 40px;
        height: 40px;
        background: #ffffff;
        border-radius: 100%;
        text-align: center;
        line-height: 50px;
        font-size: 28px;
    }
    .title span{
        color: var(--yellow);
        display: inline-block;
        font-size: 18px;
        line-height: 40px;
        margin-top: 5px;
    }
    .btn{
        width: 100%;
        padding: 20px 0;
        display: block;
        overflow: hidden;
        position: relative;
        transition: .4s all ease-in-out;
    }
    .btn::after{
        position: absolute;
        top: 15%;
        left: -100%;
        background: #dbdbdb;
        box-shadow: 0 0 20px 0 #000000;
        width: 50px;
        height: 50px;
        content: '';
        transform: rotate(45deg) translate(-50%,50%);
        transition: .4s all ease-in-out;
    }
    .btn:hover{
        background: #000000 !important;
        color: #ffffff;
    }
    .btn:hover:after{
        background: var(--yellow);
        left: 2%;
    }
    @media (min-width:300px) and (max-width:600px) {
        .qoute{
            top: 50px;
            right: 50px;
        }
        .any_question h5{
            font-size: 18px;
        }
        h3{
        font-size: 24px;
    }
    }
</style>