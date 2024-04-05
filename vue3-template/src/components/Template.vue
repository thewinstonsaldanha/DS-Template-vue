<template>
   <h1>This is template.vue output!</h1> 
   <p>{{ 'THIS IS INTERPOLATION' }}</p>
   <p>{{ 55+85 }}</p>
   <p>{{ False?'Yes':'No' }}</p>
   
   <p>Today's date is: {{ TodaysDate() }}</p>
   <p>Today's day is: {{ TodaysDay() }}</p>

</template>

<script setup>

 const TodaysDate=()=>{
    return new Date().toDateString()
}

//Todays day of the week function with output as monday, tuesday, etc.

const TodaysDay=()=>{
    return new Date().getDay()
}



</script>

<style></style>