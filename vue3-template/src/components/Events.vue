<template>
    <button @click="handleClick">Add</button>
  </template>
  
  <script setup>
  const emit= defineEmits(['someEvents', 'onClicks'])
  const handleClick = () => {
    console.log("Button clicked");
    // Emit the event to notify the parent component
    emit('someEvent');
    emit('onClicks');

  }
  </script>
  
  <style scoped>
  /* Your scoped styles here */
  </style>
  