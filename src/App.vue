<template>
  <div id="app">
    <Header/>
    <Banner/>
    <Video/>
    <RegForm/>
    <ProgramCard/>
    <Posts/>
    <BuyBanner/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Video from '@/components/Video.vue'
import RegForm from '@/components/RegForm.vue'
import ProgramCard from '@/components/ProgramCard.vue'
import Posts from '@/components/Posts.vue'
import BuyBanner from '@/components/BuyBanner.vue'
export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Video,
    RegForm,
    ProgramCard,
    Posts,
    BuyBanner
  }
}
</script>

<style lang="scss">
@import "@/styles/globals.scss";
</style>
