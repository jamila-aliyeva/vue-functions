<template>
    <button @click ="emit('notif', 'successfully saved')" :disabled="!desabled">
        save
    </button>
</template>

<script setup>
 import { defineProps, defineEmits } from 'vue';

 const etims = defineEmits(['notif'])

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