<template>
  <div class="allstick">
  <div id="navbar" ref="navbar">
    <div id="containerx">
      <a id="activeB" ref="activeB" class="activeB" @click="openSideMenu" href="javascript:void(0)"></a>
      <a @mouseover="showcat" @mouseleave="hidecat" ref="btncateg">Categories</a>
      <div id="wrapsearch">
        <div><input type="text" id="search_id" placeholder="Looking for something ?"></div>
      </div>
      <div id="searchBtn">src</div>
    </div>
  </div>
  <div class="drpdwn" ref="drpdwn" @mouseover="showcat2"  @mouseleave="hidecat2">
    <div class="drpdwncntnt" ref="drpdwncntnt">
      Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum
      Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum
      Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Lurem Ipsum Lurem
      Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum Lurem Ipsum 
    </div>
  </div>
</div>
</template>


<script>
let x = false;
export default{
  name:"NavBar",
  methods:{
    showcat(){
      x=true;
      this.$refs.drpdwn.style.height = "24vh";
      this.$refs.btncateg.style.backgroundColor = "#cd104d";
      this.$refs.btncateg.style.color = "black";
      this.$refs.drpdwncntnt.style.top = "0";
    },
    showcat2(){
      if(x==true){
        this.$refs.drpdwn.style.height = "24vh";
        this.$refs.btncateg.style.backgroundColor = "#cd104d";
        this.$refs.btncateg.style.color = "black";
        this.$refs.drpdwncntnt.style.top = "0";
      }
    },
    hidecat(){
      this.$refs.drpdwncntnt.style.top = "-24vh";
      this.$refs.drpdwn.style.height = "0vh";
      this.$refs.btncateg.style.backgroundColor = "black";
      this.$refs.btncateg.style.color ="#cd104d";
   
    },
    hidecat2(){
      x=false
      this.$refs.drpdwncntnt.style.top = "-24vh";
      this.$refs.drpdwn.style.height = "0vh";
      this.$refs.btncateg.style.backgroundColor = "black";
      this.$refs.btncateg.style.color ="#cd104d";
    }
  },
  created:
    function(){
      return
    }
}

</script>


<style >
#navbar {
  z-index: 11;
  position: fixed;
  top: 0;
  width: 100vw;
  overflow: hidden;
  background-color: /*#343A40*/black;
  box-shadow: rgba(215, 43, 118, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
  
}
#navbar a {
  cursor: pointer;
  float: left;
  display: block;
  color: #cd104d;
  text-align: center;
  padding: 2vh 3vh;
  text-decoration: none;
  font-size: 2.3vh !important;
}
#navbar a:hover {
  background-color: #cd104d;
  color: black;
}
#navbar a.activeB {
  background-color:#FFC107 !important;
  background: url(./../assets/colastream.png); /* 7952B3 */
  background-position: center;
  background-size: 95% 90%;
  background-repeat: no-repeat;
  filter:contrast(100%);
  padding-top: 2.4vh;
  padding-bottom: 2.4vh;
  height: 1.92vh !important;
  width: 16vh !important;
}
#containerx{
  display: flex;
  align-items: center;
}
#search_id{
  outline: none !important;
  box-shadow: none !important;
  background-color: black;
  width: 12vw !important;
  min-width: 180px !important;
  font-size: 2.2vh !important;
  color: grey;
  display: flex;
  justify-content: safe center;
  border: solid 2px black;
  margin-left: 1vw;
  text-decoration: none;
  transition: width 300ms;
}
#search_id:focus{
  width: 25vw !important;
}
#search_id:focus::placeholder{
  opacity: 0;
}
#wrapsearch{
  display: flex;
  height: 4.3vh;
  min-height: 17px;
  align-items: center;
  border: solid 2px #cd104d;
  border-radius:  2vh 0 0 2vh ;
  margin-left: 10px;
}
#searchBtn{
  height: 4.3vh;
  min-height: 17px;
  width: 5vh;
  background: url("./../assets/search.svg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: 80% 80%;
  border: solid 2px #cd104d;
  color: rgba(0,0,0, 0);
  padding-left: 10px;
  border-radius: 0 2vh 2vh 0;
  background-color: #cd104d;
}
#searchBtn:hover{
  cursor: pointer;
}
.mbfont{
  font-size: 1.8em !important;
  font-weight: bold !important;
}

.drpdwn{
  position: fixed;
  z-index: 10;
  top: 6.8vh;
  background-color: black;
  height: 0;
  font-size: 2.2vh !important;
  color: grey;
  margin-left: 22vh;
  width: 60vh;
  transition: height 200ms;
}
.drpdwncntnt{
  position: relative;
  top: -24vh;
  transition: top 200ms;
}
</style>
