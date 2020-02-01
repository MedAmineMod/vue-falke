<template>
  <div id="coffee-t" class="">

      <h3 >{{tableType.type}}</h3>
      <input class="ip-tsize"     v-bind:key="size.id"  v-bind:id="size.id"  v-for="size in tableType.sizes"    v-bind:value="size.label" >

  </div>
</template>

<script>
export default {
  name: 'TableSize',
  props: {
    tableType: Object
  },
  data(){
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  input {
    overflow: visible;
    height: 35px;
    text-align: left;
    background: none;
    color: rgba(255 , 255 ,255 );
    -webkit-text-fill-color: #FFFFFF;
    width: 100%;
    border-top: none;
    border-right: none;
    border-left: none;
    border-bottom: rgba(255 , 255 ,255 ) 1px solid;
    cursor: pointer;
    font-size: 14px !important;
    padding-left: 8px
  }
</style>
