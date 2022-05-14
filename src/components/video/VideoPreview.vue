<script lang='ts'>
    class Video {
        title?: string;
        alt?: string;
        link?: string;
    }
</script>
<script setup lang='ts'>
    import { defineProps } from 'vue';
    const props = defineProps({
        video: {
            type: Object,
            required: true
        }
    })
</script>

<template>
    <div class="video-player is-flex is-vcentered is-justify-content-center is-align-items-center">
        <iframe :src="props.video.link" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <p class="player-title has-text-centered ">{{props.video.title}}</p> 
    </div>
</template>
    
<style lang="scss">
    .video-player {
        position: relative;
        width: 320px;
        height: 175px;
        border-radius: 25px;
        background-color: rgba(0,0,0,.655);
        iframe {
            position: absolute;
            height: 100%;
            width: 100%;
            border-radius: 25px;
        }
        .player-title {
            position: absolute;
            bottom: 0px;
            width: 100%;
            background-color: red;
            border-radius: 0px 0px 25px 25px;
            font-size: 18px;
        }
    }
</style>