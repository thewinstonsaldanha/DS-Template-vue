<template>
     <h4>Name {{ name }}</h4>
   </template>
   
   <script setup>
   import { defineProps } from 'vue';
   
   const props = defineProps({
     name: {
       type: String,
       default: ''
     }
   });
   </script>
   