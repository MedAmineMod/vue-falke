<template lang="html">
  <div class="col-md-4 right-side" >
      <TableSize v-bind:key="tableSize.type" v-bind:tableType="tableSize" v-for="tableSize in tableSizes" />

  </div>
</template>

<script>
import TableSize from '../TableSize'
export default {
  name :"RightSide" ,
  components :{
    TableSize
  },
  props :{

   },
  data(){
    return {
      tableSizes :[
          {
            type: "COFFEE TABLE" ,
            sizes :[
            {id : "1coffee_table_50x50" , label : "50 CM x 50 CM " ,  price :  0},
            {id : "2coffee_table_50x50" , label : "80 CM x 80 CM" ,  price :  0},
            {id : "3coffee_table_50x50" , label : "70 CM x 140 CM" ,  price :  0},
            {id : "4coffee_table_50x50" , label : "ROUND TABLE Ø80 CM" ,  price :  0},
          ]
        },
        {
          type: "DINING TABLE" ,
          sizes :[
          {id : "1dinning_table_50x50" , label : "50 CM x 50 CM" ,  price :  0},
          {id : "2dinning_table_50x50" , label : "80 CM x 80 CM" ,  price :  0},
          {id : "3dinning_table_50x50" , label : "70 CM x 140 CM" ,  price :  0},
          {id : "4dinning_table_50x50" , label : "ROUND TABLE Ø80 CM" ,  price :  0},
        ]
      }

      ]
    }
  }
}
</script>

<style lang="css" scoped>
  .right-side{
    height : 100vh;
    background-color: rgba(0 , 0 , 0, 0.50);
      border : 1px solid white
  }
</style>
