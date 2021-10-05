<template>
  <div class="home">
    <h1 class="APTest">Hello World {{ student }}</h1>
    <ul class="myList">
      <li v-for="animal in animals" :key="animal">{{animal}}</li>
    </ul>
    <button v-if="isLoggedIn === false">Login</button>
    <button v-else>Logout</button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },
  data(){
    return{
    student:"Selina",
    animals:["Pig","Cow","Rooster","Monkey"],
    isLoggedIn: false,
  }
  },
  
}
</script>
<style>
.APTest{
  color:red;
}
</style>