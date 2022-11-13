<template>
<div class="playico"></div>
    
</template>
<script>
export default{
    name:"PlayIco",
}
</script>
<style>
.playico{
    z-index: 3;
    background: url('./../assets/play1.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: 0% 0%;
    width: 10vh;
    height: 10vh;
    position: relative;
    top: 3vh;
    left: 11vh;
    transition: background-size 400ms;
}
.playico:hover{
    background: url('./../assets/play2.png');
    background-repeat: no-repeat;
    background-position: center;
    cursor: pointer;
    
}
</style>