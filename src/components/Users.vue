<template>
  <div class="users">
    <h1>{{title}}</h1>
    <ul>
      <li v-for="user in users" v-on:click="user.show = !user.show">
        <h2>{{user.name}}</h2>
        <p v-show="user.show">{{user.position}}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name:'users',
  data(){
    return {
      title:"展示名字及职业",
      users:[
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
        {name:"Henry",position:"web开发",show:false},
      ]
    }
  }
}
</script>

<style scoped>
*{
  list-style: none;
  box-sizing: border-box;
}

.users{
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
}

.users ul{
  display: flex;
  flex-wrap: wrap;
  padding: 0;
}
.users ul li{
  flex-grow: 1;
  flex-basis: 200px;
  text-align: center;
  padding: 30px;
  margin: 10px;
  border: 2px solid orange;
  border-radius: 5px;
}
</style>


