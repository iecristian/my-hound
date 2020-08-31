<template>
  <div id="app">
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <app-header></app-header>
    <div class="content">
      <filters></filters>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
      <dog-detail></dog-detail>
    </div>
  </div>
</template>

<script>
import DogDetail from './components/DogDetail.vue'
import Filters from './components/Filters.vue'
import AppHeader from './components/Header.vue'

export default {
  name: 'App',
  components: {
    DogDetail,
    Filters,
    AppHeader
  },
  data(){
    return {
      info: null
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #EEEEEE;
  overflow: hidden;
  font: Poppins;
}

.content{
  max-width: 80%;
  margin-left: 120px;
  margin-right: auto;
}

@media screen and (max-width: 600px) {

    .content{
        width: 100%; 
        margin-left:auto;
        margin-right:auto;
    }

}


</style>
