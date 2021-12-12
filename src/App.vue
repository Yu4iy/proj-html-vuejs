<template>
  <div id="app">
    <Header/>
    <Banner/>
    <BannerCard/>
    <Video/>
    <RegForm/>
    <ProgramCard/>
    <Posts/>
    <BuyBanner/>
    <OtherServices/>
    <AllVideoBanner/>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import BannerCard from '@/components/BannerCard.vue'
import Video from '@/components/Video.vue'
import RegForm from '@/components/RegForm.vue'
import ProgramCard from '@/components/ProgramCard.vue'
import Posts from '@/components/Posts.vue'
import BuyBanner from '@/components/BuyBanner.vue'
import OtherServices from '@/components/OtherServices.vue'
import AllVideoBanner from '@/components/AllVideoBanner.vue'
import Footer from '@/components/Footer.vue'



export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Video,
    RegForm,
    ProgramCard,
    Posts,
    BuyBanner,
    OtherServices,
    AllVideoBanner,
    Footer,
    BannerCard
   
  }
}
</script>

<style lang="scss">
@import "@/styles/globals.scss";
</style>
