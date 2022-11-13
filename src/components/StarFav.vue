<template>
<div @click="show" ref="star" class="star" @mouseover="changeStar"></div>
</template>

<script>

export default{
    name:"StarFav",
    methods:{
        changeStar(){
            return
        },
        resetStar(){
            return
        },
        show(){
            alert("Hello World !");
        }
    }
}
</script>

<style scoped>
.star{
    z-index: 2;
    position: relative;
    width: 4vh;
    height: 4vh;
    float: right;
    margin-right: 0.4vw;
    margin-top: 1vh;
    background: url('./../assets/star1.png');
    background-size: 100% 100%;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
}
.star:hover{
    background: url('./../assets/star2.png');
    background-size: 100% 100%;
    cursor: pointer;
    
}

</style>