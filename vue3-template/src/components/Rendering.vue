<template>
    <div>

        <ul>

            <li v-for="item in data" :key="item.id">{{ item.value }}</li>
        </ul>
    </div>


</template>

<script setup>
import { ref } from 'vue';

let data = ref([
    { id: 1, value: '1' },
    { id: 2, value: '2' },
    { id: 3, value: '3' },
])

</script>