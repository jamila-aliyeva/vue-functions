<template>
  <div>
<h2>Hello World !</h2>
  </div>
</template>

<script setup>
import { watch, ref} from 'vue';
const name= ref("");

watch(name, (newValue, oldValue)=>{
  console.log(`ism o'zgardi: ${newValue} dan ${oldValue}` );
  
})

</script>

<style lang="scss" scoped>

</style>