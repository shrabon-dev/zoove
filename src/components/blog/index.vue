<template>
  <section id="blog">
    <v-container>
        <div class="title pb-10">
            <h6> <span><FeEdit/></span> Blog & Article</h6>
            <h4>Latest News and Articles</h4>
        </div>
        <v-row justify="center">

            <v-col cols="4">
                <div class="blog">
                    <div class="blg_img">
                        <picture>
                            <img :src="img" :alt="img">
                        </picture>
                       <div class="blg_dtls d-flex justify-center align-center">
                        <div class="created_by d-flex align-center align-content-center ga-3 pa-5">
                           <span> <BxSolidUser/></span> Muhammad Ali
                        </div>
                        <div class="date d-flex align-center align-content-center ga-3 pa-5">
                           <span> <HeOutlineIScheduleSchoolDateTime/></span> 19 April 24
                        </div>
                       </div>
                    </div>
                    <div class="blg_info">
                        <h5>Improve Workflow With bluecollar Construction</h5>
                        <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt. Interdum et malesuada.</p>
                        <a href="#">Read More <FaAngleRight/></a>
                    </div>
                </div>
            </v-col>
            <v-col cols="4">
                <div class="blog">
                    <div class="blg_img">
                        <picture>
                            <img :src="img2" :alt="img2">
                        </picture>
                       <div class="blg_dtls d-flex justify-center align-center">
                        <div class="created_by d-flex align-center align-content-center ga-3 pa-5">
                           <span> <BxSolidUser/></span> Muhammad Ali
                        </div>
                        <div class="date d-flex align-center align-content-center ga-3 pa-5">
                           <span> <HeOutlineIScheduleSchoolDateTime/></span> 19 April 24
                        </div>
                       </div>
                    </div>
                    <div class="blg_info">
                        <h5>Understanding Your Home’s Electrical Capacity</h5>
                        <p>Pellentesque vehicula eros neque, maximus mattis est sagittis Nulla facilisi. In sed pretium metus. Proin pretium id urna sit amet tincidunt. Interdum et malesuada.</p>
                        <a href="#">Read More <FaAngleRight/></a>
                    </div>
                </div>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
import { FeEdit } from "@kalimahapps/vue-icons";
import { BxSolidUser } from "@kalimahapps/vue-icons";
import { HeOutlineIScheduleSchoolDateTime } from "@kalimahapps/vue-icons";
import { FaAngleRight } from "@kalimahapps/vue-icons";
import blog from '../../assets/blog/blog.png'
import blog2 from '../../assets/blog/blog2.png'
export default {
    name:'BlogAndArticle',
    components:{FeEdit,BxSolidUser,HeOutlineIScheduleSchoolDateTime,FaAngleRight},
    data(){
        return{
            img:blog,
            img2:blog2,
        }
    }
}
</script>

<style scoped>
    #blog{
        padding: 100px 0;
    }
    .title{
        text-align: center;
        max-width: 600px;
        margin: 0 auto;
    }
    .blog{
        max-width: 584px;
    }
    .blg_img{
        position: relative;
        width: 100%;

    }
    .blg_img img{
        width: 100%;
        display: block;
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
    .created_by,.date{
        font-family: var(--inter);
        font-weight: 500;
        font-size: 18px;
        color: var(--main);
        background: var(--yellow);
        width: 200px;
      

    }
    .blg_dtls{
        position: absolute;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);

    }
    .created_by span,.date span{
        display: inline-flex;
        margin: 0;
        padding: 0;
    }
    .created_by{
        background: #FFC368;
    }
    .blg_info h5{
        font-family: var(--mulish);
        font-size: 30px;
        font-weight: 700;
        color: var(--main);
        padding: 55px 0 10px 0;
    }
    .blg_info p{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--sub);
    }
    .blg_info a{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);
        display: flex;
        align-items: center;
        gap: 6px;
        padding-top: 10px;
    }
    .blg_info a svg{
        display: inline-flex;
        
    }
</style>