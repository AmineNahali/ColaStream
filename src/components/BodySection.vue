<template>
  <div class="content">
    <table>
      <tr>
        <td class="halfLeft">
          <div class="filtered_search"></div>
          <div class="contentcontainer">
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
            <ComElement/>
          </div>
        </td>
        <td class="halfRight">
        </td>
      </tr>
    </table>
  </div>
</template>


<script>
import ComElement from './ComElement.vue';

export default {
  name: "BodySection",
  components:{
    ComElement
  }
}
</script>


<style>
.content {
  z-index: 1 !important;
  scale: 0.85;
  margin-top: -4vh;
}
.filtered_search{
  margin-left: 1vh;
  width: 125vh;
  height: 40vh;
  background-color: black;
  border-radius: 2vh;
  margin-right: 3.5%;
}
.halfLeft{
  width: 128vh;
}
.halfRight{
  width: 80vh;
  border-radius: 2vh;
  background-color: black;
}
.frd{
  border-radius: 2vh;
  background-color: black;
  height: 100%;
}
.frl{
  border-radius: 2vh;
  background-color: black;
  height: 100%;
}
.insideRight{
  margin-left: 4vh;
}
.contentcontainer{
  margin-top: 2vh;
  width: 128vh;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
table{
  margin-left: auto;
  margin-right: auto;
}

</style>