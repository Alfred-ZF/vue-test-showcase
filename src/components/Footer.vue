<template>
<footer>
  <p>
    {{copyright}}
  </p>
</footer>

</template>

<script>
export default {
  name:'footer',
  data(){
    return{
      copyright:"Copyright 2018 Vue Demo"
    }
    
  }
}
</script>

<style scoped>

  footer{
    width: 100%;
    background: lightgreen;
    padding: 5px;
  }

  p{
    color: #333;
    text-align: center; 
  }

</style>