<template>
    <form @submit.prevent="addData">
      <input v-model="firstName" type="text" placeholder="First Name">
      <input v-model="lastName" type="text" placeholder="Last Name">
      <input v-model="comment" type="text" placeholder="Comment">
      <button type="submit">ADD</button>
    </form>
</template>

<script>
export default {
    components:{
      // FriendCard
    },
    emits: "add-data",
    data(){
      return {
        firstName: "",
        lastName: "",
        comment: "",
      }
    },
    
    methods: {
      addData(){
        this.$emit('add-data', this.firstName, this.lastName, this.comment)
      }
    }

  }
</script>

<style scoped>
    form{
    padding: 10px;
    margin-top: 200px;
    background: #fff;
    width: 500px;
    margin: auto;
    box-sizing: border-box;
    border-radius: 3px;
    }

    form input{
    margin: 10px;
    width: 90%;
    padding: 10px;
    border-radius: 3px;
    }
    form button{
    box-sizing: border-box;
    /* margin: 10px; */
    width: 95%;
    padding: 10px;
    border-radius: 3px;
    margin-left: 10px;
    font-weight: bold;
    color: #fff;
    background: rgb(170, 160, 160);
    }

</style>