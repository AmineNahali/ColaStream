<template>
    <div class="ModElementContainer">
        <StarFav/>
        <p class="movieTitle">Bladerunner 2049</p>
        <p class="movieYear">(2017)</p>
        <div class="movieTag">Movie</div>
        <PlayIco/>
        
    </div>
</template>

<script>
import StarFav from './StarFav.vue';
import PlayIco from './PlayIco.vue';
export default{
    name:"ComElement",
    components:{
        StarFav,
        PlayIco
    }
}
</script>

<style>
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
    margin-left: 15px;
    margin-top: 15px;
    position: relative;
    top: 0;
    transition: top 600ms,background-size 600ms,box-shadow 600ms;
}
.ModElementContainer:hover{
    background-position: center;
    background-size: 120% 120%;
    background-blend-mode: color ;
    box-shadow: rgba(50, 50, 93, 0.9) 0px 13px 3px -5px, rgba(0, 0, 0, 0.7) 0px 8px 3px -8px;
    top: -5px;
}
.ModElementContainer:hover .playico{
    background-repeat: no-repeat;
    background-size: 100% 100%;
    
    transition: background-size 400ms;
}
.movieTag{
    font-size: 2.5vh !important;
    text-align: center;
    width: 4.2vw;
    height: 2.8vh;
    font-weight: bold;
    background-color: #FF1E00;
    position: relative;
    bottom: -70%;
    left: 2%;
    border-radius: 5px;
    cursor:default;
}
.movieTitle{
    color: aliceblue;
    font-size: 2.2vh !important;
    text-shadow: 2px 2px 8px #000;
    text-align: left;
    margin-left: 0.4vw;
    position: relative;
    top: -1vh;
    cursor:default;
}
.movieYear{
    color: aliceblue;
    font-size: 1.8vh !important;
    text-shadow: 2px 2px 8px #000;
    text-align: left;
    margin-left: 0.4vw;
    margin-top: -2.6vh;
    cursor:default;
}
</style>