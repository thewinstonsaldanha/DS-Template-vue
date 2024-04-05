<template>
<h1>Primary button component</h1>
<button @click="counter">Click</button>
</template>

<script setup>
import { onBeforeMount, onMounted , onBeforeUpdate, onUpdated, onUnmounted} from 'vue';

const count= ref(0);
const counter = ()=>{
    count.value++;
}
onBeforeMount(() => {
  console.log('onBeforeMount');
});

onMounted(() => {
  console.log('onMounted');
});


onBeforeUpdate(()=> {
    console.log('onBeforeUpdate')
})

onUpdated(()=>{
    console.log('onUpdated')
})
</script>

<style scoped>


</style>