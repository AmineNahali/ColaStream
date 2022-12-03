<template>
<div @click="addToFavs" ref="star" class="star"></div>
</template>

<script>
export default{
    name:"StarFav",
    methods:{
        addToFavs(){
            if(this.$refs.star.classList[1] == "permenantstar"){
                this.$refs.star.classList.remove("permenantstar");
            }
            else{
                this.$refs.star.classList.add("permenantstar");
            }

        }
    }
}
</script>

<style>
.star{
    z-index: 3;
    position: relative;
    width: 4vh;
    height: 4vh;
    float: right;
    margin-right: 2.8vh;
    margin-top: 2.8vh;
    background: url('./../assets/star1.png');
    background-size: 100% 100%;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
}
.star:hover{
    background-size: 100% 100%;
    cursor: pointer;
    
}
.permenantstar{
    z-index: 3;
    position: relative;
    width: 4vh;
    height: 4vh;
    float: right;
    margin-right: 2.8vh;
    margin-top: 2.8vh;
    background: url('./../assets/star2.png');
    background-size: 100% 100%;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
}

</style>