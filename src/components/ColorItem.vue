<template lang="html">
  <div class="col-6 " style="text-align :  center ">
    <div v-bind:id="item.id" class="color-box">
      <img v-bind:src="item.img">
      <h3>{{item.color}}</h3>
    </div>
  </div>

</template>

<script>
export default {
  name : 'ColorItem' ,
  props:{
    item : Object
  }
}
</script>

<style lang="css" scoped>
img {
  max-height : 150px ;
}
h3 {
  font-size : 14px 
}
</style>
