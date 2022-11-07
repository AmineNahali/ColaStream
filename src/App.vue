<template>
  <div class="floaties">
    <NavBar/>
    <SideMenu/>
  </div>
  <BodySection/>
</template>

<script>
//import HeaderSection from './components/HeaderSection.vue';
import BodySection from './components/BodySection.vue';
import NavBar from './components/NavBar.vue';
import SideMenu from './components/SideMenu.vue';


export default {
  name: 'App',
  components: {
    BodySection,
    NavBar,
    SideMenu
  }
}
</script>

<style>
.floaties{
  display: inline-block;
  justify-content:center;
}
</style>
