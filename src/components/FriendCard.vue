<template>
    <section>
      <div class="card">
        <div class="name">
            <h3>{{list.firstName}} </h3>
            <h3>{{list.lastName}} </h3>
        </div>
        <p>{{list.comment}}</p>
        <div class="skill">
          <friend-skill v-for="skill of list.skills" :key="skill" :skill="skill"></friend-skill>
        </div>  
        <button>Delete</button>
      </div>
    </section>
</template>

<script>
    export default {
      // props: ["lists"],
      props: {
        list:Object,
      },

      methods: {
        deleteItem(listItems, index){
          console.log(listItems)
          listItems.splice(index, 1);
        }
      }
    }
</script>


<style>
section{
  margin-top: 20px;
}
.card{
  border-radius: 3px;
  padding: 5px 10px;
  background: rgb(255, 255, 255);
  width: 500px;
  margin: auto;
  box-sizing: border-box;
  margin-top: 10px;
  box-shadow: rgba(0, 0, 0, 0.15) 0px 5px 15px 0px;
}
.name{
    display: flex;
    
}
.name h3{
    margin-right: 15px;
}
button{
  width: 100%;
  padding: 10px 20px;
  background: rgb(226, 76, 76);
  border:none;
  border-radius: 5px;
  color: white; 
}
.skill{
  display: flex;
  flex-wrap: wrap;
}
</style>