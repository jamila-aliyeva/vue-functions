<template>
  <div class="wrapper">
   <div class="card">
   <img src="https://picsum.photos/id/142/300/270" alt="sm photo">
   <div class="card-body">
    <h1 class="card-title">Card 1</h1>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit!</p>
   </div>
   </div>
  </div>
</template>

<script setup>


</script>

<style  lang="scss" scoped>
.wrapper{
padding: 20px;
border: 1px solid black;
}
.card{
  width: 200px;
  height: 290px;
  background-color: #fff;
  box-shadow: 0 0 20px silver;
  font-family: sans-serif;
  cursor: pointer;

  img{
    width: 100%;
    height: 170px;
  }
  &-body{
    padding-inline: 10px;
    
    h1{
      font-size: 19px;
    }
  }
}

</style>