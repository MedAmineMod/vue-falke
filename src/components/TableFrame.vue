<template lang="html">
  <div class="">


  <div class=" compo-title ">
      <h2>FRAME COLOR </h2>
  </div>
  <div  id="" class="" style= "display : flex ;  flex-wrap:wrap;     justify-content:space-between;">
    <!-- <h3 style= "text-align : left">COFFEE TABLE</h3> -->
    <div class="container-fluid">
      <div class="row">
        <ColorItem v-bind:key="item.id" v-bind:item="item" v-for="item in tableFrame" />
      </div>
    </div>

  </div>
  </div>
</template>

<script>
import  ColorItem from './ColorItem'
export default {
  name :  "TableFrame" ,
  components :{
    ColorItem
  },
  props:{

  },
  data() {
    return {
      tableFrame :[
        {color : "WHITE" , img :require("../assets/miamiwhite.jpg") ,  id : 'fr-col-white'},
        {color : "STAINLESS STEEL" , img :require("../assets/steel-flake.jpg"),  id : 'fr-col-ststeel'},
        {color : "BLACK" , img :require("../assets/iconicblack.jpg") , id : 'fr-col-black'},
        {color : "BRASS" , img :require("../assets/brass.jpg"),  id : 'fr-col-brass'},
      ]
      }
    }
  }

</script>

<style lang="css" scoped>
.compo-title {
    text-align: center;
    height: 110px;
    padding: 35px 0px 35px 0px;
}

</style>
