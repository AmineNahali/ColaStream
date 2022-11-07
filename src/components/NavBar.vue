<template>
  <div id="navbar" ref="navbar">
    <div id="containerx">
        <a id="activeB" ref="activeB" class="activeB" @click="openSideMenu" href="javascript:void(0)">
          <div class="mbfont">≡</div>
        </a>
        <a href="javascript:void(0)">New</a>
        <a href="javascript:void(0)">Popular</a>
        <a href="javascript:void(0)">Categories</a>
        <div id="wrapsearch">
            <div><input type="text" id="search_id" placeholder="Looking for something ?"></div>
            <div id="search_btn">
                <svg id="search_holder" style="width: 32px;height: 32px;" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 50 50">
                    <g id="surface150425">
                        <path style=" stroke:none;fill-rule:nonzero;fill:rgb(100%,75.686276%,2.745098%);fill-opacity:1;" d="M 21 3 C 11.601562 3 4 10.601562 4 20 C 4 29.398438 11.601562 37 21 37 C 24.355469 37 27.460938 36.015625 30.09375 34.34375 L 42.375 46.625 L 46.625 42.375 L 34.5 30.28125 C 36.679688 27.421875 38 23.878906 38 20 C 38 10.601562 30.398438 3 21 3 Z M 21 7 C 28.199219 7 34 12.800781 34 20 C 34 27.199219 28.199219 33 21 33 C 13.800781 33 8 27.199219 8 20 C 8 12.800781 13.800781 7 21 7 Z M 21 7 "/>
                    </g>
                </svg>
            </div>
        </div>
    </div>
  </div>
  <div class="sidenav" ref="mySidenav">
    <span class="SideNavClose" @click="closeSideMenu">&times;</span>
    <a href="javascript:void(0)" class="SideNavItem">Link 1</a>
    <a href="javascript:void(0)" class="SideNavItem">Link 2</a>
    <a href="javascript:void(0)" class="SideNavItem">Link 3</a>
  </div>
</template>


<script>
export default{
  name:"NavBar",
  methods:{
    openSideMenu() {
      this.$refs.mySidenav.style.width = "250px";
    },
    closeSideMenu() {
      this.$refs.mySidenav.style.width = "0";
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
  z-index: 10;
  position: fixed;
  top: 0;
  width: 100%;
  overflow: hidden;
  background-color: #343A40;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
}
#navbar a {
  float: left;
  display: block;
  color: #FFC107;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}
#navbar a:hover {
  background-color: #E1E8EB;
  color: black;
}
#navbar a.activeB {
    background-color:#FFC107 !important;
    color: black !important;
    height: 20px !important;
    width: 22px !important;
    display: flex !important;
    align-items: center !important; 
    justify-content: center !important;
}
#navbar a.activeB:hover {
  background-color: #E1E8EB !important;
  color: black !important;
}
#containerx{
  display: flex;
  align-items: center;
}
#search_id{
  outline: none !important;
  box-shadow: none !important;
  background-color: #343A40;
  height: 26px;
  width: 25vw !important;
  font-size: 17px;
  color: #FFC107;
  display: flex;
  justify-content: safe center;
  border: solid 2px #343A40;
  margin-left: 4px;
  text-decoration: none;
}
#search_btn{
  height: 32px;
  width: 32px;
  position: relative;
  left: 0.3rem;
  border-radius: 5px;
  margin-right: 10px;
}
#search_btn:hover{
  cursor: pointer;
}
#wrapsearch{
  display: flex;
  align-items: center;
  border: solid 2px #FFC107;
  border-radius: 5px;
  height: fit-content;
  margin-left: 10px;
}
/* Menu Button */
.mbfont{
    font-size: 1.8em !important;
    font-weight: bold !important;
}
.sidenav {
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 12;
  top: 0;
  left: 0;
  background-color: #FFC107;
  overflow-x: hidden;
  transition: 0.5s;
  padding-top: 60px;
}
.SideNavItem{
  width: 100%;
  border: none;
  text-align: left;
  background-color: rgba(0, 0, 0, 0);
}
.SideNavItem:hover{
  background-color: #E1E8EB;
}
.sidenav .SideNavItem {
  padding: 8px 8px 8px 32px;
  text-decoration: none;
  font-size: 14px !important;
  color: black;
  display: block;
  transition: 0.3s;
}
.SideNavClose{
  font-size: 40px;
  position:absolute;
  top: 0;
  right: 0;
  margin-right: 10px;

}
.SideNavClose:hover{
  cursor: pointer;
  color: #E1E8EB;
}
</style>
