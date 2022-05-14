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
  <div class="columns">
    <div class="column is-5 is-offset-7 ">
      <div class="columns is-multiline">
        <div class="column is-5" v-for="(video, index) in state.videos" :key="index">
          <VideoPreviewVue :video="video"/>
        </div>
      </div>
    </div>
  </div>
</template>
