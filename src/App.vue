<template>
  <div class="wrapper">
  <Card v-for="el in 4" :key="el"/>
  </div>
</template>

<script setup>
import Card from "./components/card/index.vue"

</script>

<style  lang="scss" scoped>
.wrapper{
    padding: 20px;
    border: 1px solid black;
    display: flex;
    justify-content: space-between;
    gap: 12px;
}


</style>