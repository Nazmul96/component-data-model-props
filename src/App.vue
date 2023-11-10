<script setup>
 import Radio from './components/Radio.vue'
 import {ref} from 'vue';
 const fruit = ref('banana');

</script>

<template>
     <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          fruit name: {{ fruit }}<br/>
        </div><br><br>

        <div class="mt-10">
            <label> Your favorite fruit</label> <br />
            <Radio v-model="fruit" label="Apple" value="apple"/>
            <Radio v-model="fruit" label="Banana" value="banana"/>
            <Radio v-model="fruit" label="Orange" value="orange"/>
        </div>
  
    </div>  
</template>

<style scoped>

</style>
