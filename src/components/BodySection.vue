<template>
  <div class="content">
  <div class="contentcontainer">
    <br>
    <table>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      <tr>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
        <td><ComElement/></td>
      </tr>
      
    </table>
  </div>
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
  background-color: #E1E8EB;
  display: flex;
  justify-content: center;
}
.sticky + .content {
  padding-top: 60px;
}
.contentcontainer{
  margin-top: 6vh;
}
</style>