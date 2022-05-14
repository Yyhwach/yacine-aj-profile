<template>
    <h1 class="yacine">Yacine</h1>
    <h1 class="ajouaou">Ajouaou</h1>
</template>
    
<script setup lang='ts'>
    
</script>
    
<style scoped lang="scss">
    h1 {
        &.yacine {
            left: 0px;
            top: 0px;
        }
        &.ajouaou {
            left: 10px;
            top: 55%;
        }
        width: 100%;
        position: absolute;
        opacity: 0.29;
        background: linear-gradient(180deg, #33afff 0%, rgba(0,34,57,0) 100%);
        background-clip: text;
        -webkit-background-clip: text;
        -moz-background-clip: text;
        -webkit-text-fill-color: transparent; 
        -moz-text-fill-color: transparent;
        font-size: 288px;
        font-weight: 900;
        line-height: 349px;
        text-align: center;
        z-index: 1;
    }
</style>