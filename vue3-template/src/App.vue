<template>
    <div class="main-container">
        <h1>Hello Vue</h1>
        <!-- <Button /> -->
        <!-- <Template /> -->
        <!-- <Counter /> -->
         <!-- <Bind /> -->
        <!-- <Rendering />  -->
        <!-- <Conditional /> -->
        <!-- <Props /> -->
        <!-- <styling /> -->
        <!-- <twowaybinding /> -->
        <!-- <clicking /> -->
        <!-- <Events @someEvent="callBack" @onClicks="function1" /> -->
        <!-- <Watcher /> -->
        <LifeCycleHook />
       


    </div>
</template>

<script setup>
    import Button from './components/Button.vue';
    import Template from './components/Template.vue';
    import Counter from './components/Counter.vue';
    import Bind from './components/BindingVue.vue';
    import Rendering from './components/Rendering.vue';
    import Conditional from './components/Conditional.vue';
    import Props from './components/Props.vue'
    import styling from './components/v-html.vue'
    import twowaybinding from './components/twowaybinding.vue'
    import clicking from './components/Clicking.vue'
    import Events from './components/Events.vue'
    import Watcher from './components/watcher.vue'
    import LifeCycleHook from './components/LifeCycleHook.vue';


    const callBack=() =>{
        console.log('Callback is running | Parent Catched')
    }
    const function1=() =>{
        console.log('function 1 is running | Child Catched')
    }

   

</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap');

    body {
        margin: 0px;
        height: 100vh;
        font-family: 'Roboto', sans-serif;
    }

    #app {
        height: 100%;
    }

    .main-container {
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
</style>
