<template>
    <form action="">
      <input type="text" placeholder="First Name">
      <input type="text" placeholder="Last Name">
      <input type="text" placeholder="Comment">
      <button type="button">ADD</button>
    </form>
</template>


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