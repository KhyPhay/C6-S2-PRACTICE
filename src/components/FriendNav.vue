<template>
  <nav>
      <ul class="nav">
        <li>HOME</li>
        <li>ABOUT</li>
        <li>SERVICES</li>
        <li>HELP</li>
      </ul>
    </nav>
</template>

<script>
// export default {
 
// }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
nav{
  position: sticky;
  z-index: 20;
  top: -5px;
}
.nav {
  box-sizing: border-box;
  margin: 0;
  display: flex;
  list-style: none;
  background:rgb(233, 131, 131);
  width: 100%;  
  padding: 10px;
  color: white;
  margin-bottom: 10px;
}

.nav li{
  margin: 0 10px;
}

</style>
