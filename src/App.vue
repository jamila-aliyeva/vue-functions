<template>
  <div class="wrapper">
  <Card v-for="item in cardData" :data="item" :key="item.id" />
  </div>
</template>

<script setup>
import { ref } from "vue";
import Card from "./components/card/index.vue";

const cardData=ref([
 {
  img:"https://picsum.photos/id/300/300/300",
    title:"Card title 1", 
    description: "lorem ipsum lorem 1", 
    isBuy:"true"
 }, 
 {
  img:"https://picsum.photos/id/302/300/300",
    title:"Card title 2", 
    description: "lorem ipsum lorem 2",
    isBuy:"false"
 }, {
  img:"https://picsum.photos/id/306/300/300",
    title:"Card title 3", 
    description: "lorem ipsum lorem 3",
    isBuy:"false"
 }
 , {
  img:"https://picsum.photos/id/304/300/300",
    title:"Card title 4", 
    description: "lorem ipsum lorem 4",
    isBuy:"true"
 }
])

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