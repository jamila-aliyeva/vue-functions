<template>
    <button :disabled="!desabled">
        button
    </button>
</template>

<script setup>
 import { defineProps } from 'vue';

 const props=defineProps({
    desabled:{
        type: Boolean, 
        required: true, 
        default: true
    }
 })
</script>
 
<style lang="scss" scoped>
button{
    padding: 6px 12px;
    border-radius: 4px;
    &:focus{
        border: 2px solid green;
        background-color:green ;
        color: #fff;
    }
    &:hover{
        filter: brightness(0.7);
    }
 }
</style>