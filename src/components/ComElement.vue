<template>
    <div class="ModElementContainer">
        
    </div>
</template>


<script>
</script>


<style scoped>
.ModElementContainer{
    z-index: 2;
    height: 40vh;
    width: 30vh;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    border: solid 2px #FFC107;
    border-radius: 10px;
    background-image: url("./../assets/1.jpg");
    background-size: 100% 100%;
    background-position: center;
    transition: background-size 600ms ;
    margin-left: 15px;
    margin-top: 15px;
}
.ModElementContainer:hover{
    background-position: center;
    background-size: 120% 120%;
    transition: 400ms;
}
</style>