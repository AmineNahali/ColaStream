<template>
<div ref="playico" class="playico"></div>
    
</template>
<script>
export default{
    name:"PlayIco",
}
</script>
<style>
.playico{
    opacity: 0.001;
    z-index: 3;
    background: url('./../assets/play1.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: 40% 40%;
    width: 10vh;
    height: 10vh;
    position: relative;
    top: 9.6vh;
    left: 10vh;
    transition: background-size 200ms;
}
</style>