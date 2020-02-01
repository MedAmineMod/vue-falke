<template>
  <div id="app" class="container-fluid">
      <div class="row">
        <leftSide/>

        <rightSide/>
      </div>
  </div>
</template>

<script>
import leftSide from './components/layouts/leftSide'
import RightSide from './components/layouts/RightSide'
// import TableTopMat from './components/TableTopMat'

export default {
  name: 'app',
  components: {
    RightSide ,
    leftSide ,
    // TableTopMat
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: White;

}
div {

}
.container-fluid{
  height  : 100vh
}
</style>
