<!-- <template>
    <p>Watcher</p>
    <button @click="incrementCounter">Click - {{ count }}</button>
  </template>
  
  <script setup>
  import { ref, watch } from 'vue';
  
  const count = ref(0);
  
  const incrementCounter = () => {
    count.value++;
  };
  
  watch(count, (newVal, oldVal) => {
    console.log("The old value is === ", oldVal);
    console.log("The new value is === ", newVal);
  });
  </script>
  
  <style scoped>
  /* Your scoped styles here */
  </style>
   -->



   <template>
    <h1>Watcher</h1>
    <p>
        Ask a yes/no question
        <input v-model="question" />
    </p>
    <p>{{ answer }}</p>

   </template>

   <script setup>

   import {ref, watch} from 'vue'

   const question= ref(' ');
   const answer= ref('Questions contain a qustion mark?');


watch(question, async(newQuestion, oldQuestion) =>{
    if(newQuestion.indexOf('?')> -1){
        answer.value = 'Thinking';
        try{
            const res= await fetch(
                'https://yesno.wtf/api'
            );
            answer.value=(await res.json()).answer;
          
        } catch(error){
            answer.value = 'Nope' + error;
        }
    }
})
</script>

<style scoped>

</style>