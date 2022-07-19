<template>
<div id="app">
  <FriendNav/>
  <FriendForm/>
  <FriendCard/>
</div>
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
import FriendNav from './components/FriendNav.vue'
import FriendForm from './components/FriendForm.vue'
import FriendCard from './components/FriendCard.vue'
export default {
  name: 'App',
  components: {
    FriendNav,
    FriendForm,
    FriendCard
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
