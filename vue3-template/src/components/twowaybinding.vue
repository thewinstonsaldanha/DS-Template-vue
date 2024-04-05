<template>
    <input type="text" v-model="name"/>
    <p>{{ name }}</p>
</template>

<script setup>
import {ref} from 'vue'


let name= ref(
    'Andrew'
)
</script>

<style scoped>


</style>