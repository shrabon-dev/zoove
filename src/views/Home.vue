<template>
   <HeaderSection/>
   <NavBar/>
   <HeroSection/>
   <FutureComp/>
   <MainService/>
   <ServiceComp/>
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
export default {
    name:'HomePage',
    components:{
        HeaderSection,NavBar,HeroSection,FooterSection,SubscribeComp,FutureComp,ServiceComp,MainService
    }

}
</script>

<style>

</style>