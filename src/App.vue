<template>
  <NavBar/>
  <BodySection/>
</template>

<script>
//import HeaderSection from './components/HeaderSection.vue';
import BodySection from './components/BodySection.vue';
import NavBar from './components/NavBar.vue';

export default {
  name: 'App',
  components: {
    BodySection,
    NavBar,
  }
}
</script>

<style>

</style>
