<template>
     <div class="card" >
   <img :src="props.data.img" alt="sm photo">
   <div class="card-body">
    <h1 class="card-title">{{ props.data.title }}</h1>
    <p>{{ props.data.description }}</p> 
    <Button @notif="recivedData" />
   </div>
   </div>
</template>

<script setup>
import { defineProps} from 'vue';
import Button from "../button/index.vue"

// const props=defineProps(['title', 'body', 'img']) first way

const recivedData=(massege)=>{
  emit('notif', massege)
  
}
const emit=defineEmits(['notif'])

const props=defineProps({
  data:{
   type: Object, 
   required: true,
   default:()=>({
     title:'default value', 
     description: 'default body', 
     img: 'https://picsum.photos/id/304/309/300',
     isBuy: false
   })
  
  }
})
</script>

<style lang="scss" scoped src="./style.scss">

</style>