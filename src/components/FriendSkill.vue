<template>
    <span>{{skill}}</span>
</template>



<script>
    export default{
        props:{
            skill:String,
        }
    }

</script>

<style scoped>
    span {
        border-radius: 5px;
        background:rgb(233, 131, 131);
        padding: 10px 20px;
        margin: 10px;
        color: white;
    }
</style>
