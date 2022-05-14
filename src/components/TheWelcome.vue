<script setup lang="ts">
  import { reactive } from 'vue';
  import VideoPreviewVue from './video/VideoPreview.vue';
  
  const state = reactive({
    videos: [
      {alt: "", title: "Roulette", link: "https://www.youtube-nocookie.com/embed/4U2eWftWPCY?control=0"},
      {alt: "", title: "Roulette", link: "https://www.youtube-nocookie.com/embed/Lt--i8BGN3A?control=0"}, 
      {alt: "", title: "Roulette", link: "https://www.youtube-nocookie.com/embed/kSqGFhpuxDM?control=0"},
      {alt: "", title: "Roulette", link: "https://www.youtube-nocookie.com/embed/3GWgyDO4c1w?control=0"}]
  })
</script>

<template>
  <div class="hero banner is-primary">
    <div class="columns">
      <div class="column is-5 is-offset-7 ">
        <div class="columns is-multiline">
          <div class="column is-5" v-for="(video, index) in state.videos" :key="index">
            <VideoPreviewVue :video="video"/>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="hero subbanner">
    <div class="columns">
      <div class="column is-6 has-background-grey"></div>
      <div class="column is-6 has-background-grey-light"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .hero {
    &.banner {
      background-color: #FFC884;
      height: calc(60vh - 25px);
    }
    &.subbanner {
      background-color: white;
      height: calc(40vh - 25px);
    }
  }
</style>