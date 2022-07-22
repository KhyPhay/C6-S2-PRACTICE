<template>
<div id="app">
  <FriendNav/>
  <FriendForm @add-data="addFriend" />
  <friend-card v-for="list of lists" :key="list" :list="list" :skills="skills"> </friend-card>
</div>
</template>

<script>
import FriendNav from './components/FriendNav.vue'
import FriendForm from './components/FriendForm.vue'
export default {
  name: 'App',
  components: {
    FriendNav,
    FriendForm,
  },
  data(){
    return {
      lists : [
        {firstName:"khy", lastName:"Phat", comment:"HelloWorld", skills:["PYTHON", "JAVASCRIPT","JAVA", "NODE JS", "LARAVEL", "OOP"]},

      ],
    }
  },

  methods: {
    addFriend(fname, lname, comment){
      let friend = {firstName:fname, lastName:lname, comment:comment, skills:["PYTHON", "JAVASCRIPT","JAVA", "NODE JS", "LARAVEL", "OOP"]}
      this.lists.push(friend);
    }
  }
}
</script>

<style>
body{
  margin: 0;
  padding: 0;
  background: rgb(221, 221, 221);
}
</style>
