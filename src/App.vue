<template>
  <div id="app">
    <Header/>
    <Banner/>
    <Video/>
    <RegForm/>
    <ProgramCard/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Video from '@/components/Video.vue'
import RegForm from '@/components/RegForm.vue'
import ProgramCard from '@/components/ProgramCard.vue'
export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Video,
    RegForm,
    ProgramCard
  }
}
</script>

<style lang="scss">
@import "@/styles/globals.scss";
</style>
