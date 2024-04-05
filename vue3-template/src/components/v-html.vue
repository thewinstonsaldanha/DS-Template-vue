<template>
    <p>Hello</p>

    <p>

        <span v-html="span_tag"></span>
    </p>


</template>

<script setup>

import {ref} from 'vue';

// let span_tag= ref('<span style="color: red">I am using span </span>);

let span_tag = ref('<span style="color: red">I am using span</span>');
</script>


<style scoped>

</style>