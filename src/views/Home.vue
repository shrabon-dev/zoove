<template>
   <HeaderSection/>
   <NavBar/>
   <HeroSection/>
   <FutureComp/>
   <MainService/>
   <ServiceComp/>
   <WhyChooseUs/>
   <GalleryComp/>
   <TestimonialComp/>
   <PricePlan/>
   <OurClient/>
   <BlogAndArticle/>
   <SubscribeComp/>
   <FooterSection/>
</template>

<script>
import HeaderSection from '../components/header/index.vue';
import NavBar from '../components/navs/index.vue';
import HeroSection from '../components/hero/index.vue';
import FooterSection from '../components/footer/index.vue';
import FutureComp from '../components/future/index.vue';
import SubscribeComp from '../components/subscribe/index.vue';
import ServiceComp from '../components/services/index.vue';
import MainService from '../components/main_service/index.vue';
import WhyChooseUs from '../components/why_choose_us/index.vue';
import GalleryComp from '../components/gallery/index.vue';
import TestimonialComp from '../components/testimonial/index.vue'
import PricePlan from '../components/price_plan/index.vue'
import BlogAndArticle from '../components/blog/index.vue'
import OurClient from '../components/client/index.vue'
export default {
    name:'HomePage',
    components:{
        HeaderSection,NavBar,HeroSection,FooterSection,SubscribeComp,FutureComp,ServiceComp,MainService,WhyChooseUs,GalleryComp,TestimonialComp,PricePlan,BlogAndArticle,OurClient
    }

}
</script>

<style>

</style>