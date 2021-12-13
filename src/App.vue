<template>
  <div id="app">
    <Header :headerData = "headerData"/>
    <Banner/>
    <BannerCard/>
    <Video/>
    <RegForm/>
    <ProgramCard/>
    <Posts :posts = "posts"/>
    <BuyBanner/>
    <OtherServices/>
    <AllVideoBanner/>
    <Footer 
    :footerData = "footerData"
    :posts = "posts"
    />
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

import data from "./data";


export default {
  name: 'App',
  data() {
    return {
      posts:[],
      headerData:[],
      footerData:{},
      datas:{},
    };
	},
  mounted(){
    this.getData()
    this.getHeader()  
    this.getFooter()
    this.getPosts()
    },
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
    BannerCard,
    
   
  },
  methods:  {
    getData(){
      this.datas = data
    },
    getHeader(){
      this.headerData = this.datas.header
    },
    getFooter(){
      this.footerData = this.datas.footer
    },
    getPosts(){
      this.posts = this.datas.posts
      
    },

  }
}
</script>

<style lang="scss">
@import "@/styles/globals.scss";
</style>
