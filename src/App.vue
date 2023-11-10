<script setup>
 import Checkbox from './components/Checkbox.vue'
 import {ref} from 'vue';
 const taskDone = ref(false);

</script>

<template>
     <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          Task Done: {{ taskDone }}<br/>
        </div><br><br>

        <div class="mt-10">
            <Checkbox label="Complete yout task" v-model="taskDone"/>
        </div>
  
    </div>  
</template>

<style scoped>

</style>
