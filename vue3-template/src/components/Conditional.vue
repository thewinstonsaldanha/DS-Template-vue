<template>
    
    <div>
  <!-- <p>Hello</p>
  <h2 v-if="flag">Hello again</h2>
  <h2 v-else>Else is running</h2> -->

  <button @click="onClick">Click</button>
  <!-- <p v-if="flag">Clicked</p> -->

  <p v-show="flag">Clicked</p>


    </div>
</template>

<script setup>
import {ref} from 'vue';

let flag= ref(false);

const onClick = () => {
  flag.value =!flag.value;
}

</script>