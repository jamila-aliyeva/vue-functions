<template>
  <div>
<h2>Hello World !</h2>
<input type="text" placeholder="ismingizni kiriting" v-model="name">
  </div>
</template>

<script setup>
import { watch, watchEffect, ref} from 'vue';
const name= ref("Jamila");

watch(name, (newValue, oldValue)=>{
  console.log(`ism o'zgardi: ${newValue} dan ${oldValue}` );
})

watchEffect(()=>{
  console.log("effect:", name.value);
  
})
console.log("no effect:", name.value);

</script>

<style lang="scss" scoped>

</style>