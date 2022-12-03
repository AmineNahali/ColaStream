<template>
<div class="ModElementContainerWrapper" >
   <StarFav/>
   <div class="contentplustitle" @click="clicked">
        <div class="ModElementContainer"> 
            <!--<div class="filter">-->
            <div class="resolution">HD</div>
            <PlayIco/>
            <!--</div>-->
        </div>
        <div class="movieTitle">Bladerunner 2049</div>
    </div>
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
    },
    methods:{
        clicked(){
            alert("hey")
        },
    }
}
</script>

<style>
.ModElementContainerWrapper{
    cursor: pointer;
    box-sizing: border-box;   
}
.ModElementContainer{
    margin-left: 2vh;
    margin-right: 2vh;
    margin-top: 2vh;
    z-index: 2;
    height: 38vh;
    width: 28vh;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    /*border: solid 3px #cd104d;*/
    border-radius: 1vh;
    background: url("./../assets/2.jpg"), rgba(0, 0, 0, 0.4);
    background-size: 100% 100%;
    background-position: center;
    transition: background-size 600ms,box-shadow 600ms;
}
.ModElementContainerWrapper:hover .ModElementContainer{
    background-position: center;
    background-size: 120% 120%;
    background-blend-mode: hue;
}
.ModElementContainerWrapper:hover .ModElementContainer .playico{
    opacity: 1;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    transition: background-size 400ms opacity 200ms;
}
.ModElementContainerWrapper:hover .movieTitle{
    color: #cd104d;
}
.resolution{
    z-index: 2.2;
    font-size: 2.4vh !important;
    text-align: center;
    width: 5vh;
    height: 2.8vh;
    font-weight: bold;
    background-color:#FFC107;
    border: solid 1px #FFC107;
    padding-top: 2px;
    border-radius: 1vh 0vh 1vh 0vh;
    cursor: pointer;
    position: relative;
    top: -0.5vh;
    left: -0.5vh;
}
.movieTitle{
    z-index: 2;
    color: whitesmoke;
    font-size: 2.2vh !important;
    text-shadow: 2px 2px 8px #000;
    text-align: center;
    margin-top: 2vh;
    margin-bottom: 2vh;
    margin-left: 0.4vw;
    cursor:pointer;
}
.ModElementContainerWrapper{
    width: fit-content !important;
}
.contentplustitle{
    width: max-content;
    height: max-content;
    display: flexbox;
}
</style>