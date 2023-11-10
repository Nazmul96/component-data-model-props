<script setup>
 import TextComponent from './components/TextComponent.vue'
 import {ref} from 'vue';
 const fname = ref('nazmul');
 const lname = ref('hossain');
</script>

<template>
     <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          Original Name: {{ fname }}<br/>
          Original email: {{ lname }}<br/>
        </div><br><br>

        <div class="mt-10">
            <text-component v-model:fname="fname" v-model:lname="lname"/>
        </div>
  
    </div>  
</template>

<style scoped>

</style>
