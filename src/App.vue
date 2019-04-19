<template>
  <div id="app">
    <vue-app-header></vue-app-header>
    <users></users>    
    <vue-app-footer></vue-app-footer>
    <!-- <img src="./assets/logo.png">
    <HelloWorld/> -->
  </div>
</template>

<script>
// import HeloWorld from './components/HelloWorld'
import Users from './components/Users'
import Footer from './components/Footer'
import Header from './components/Header'

export default {
  name: 'App',
  data(){
    return{
      title:"这是我的第一个 vue 项目"
    }
  },
  components:{
    'users': Users,
    'vue-app-footer': Footer,
    'vue-app-header': Header
  }
  // components: {
  //   HelloWorld
  // }
}
</script>

<style scoped>
/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */

h1{
  color: purple;
}
</style>
