<script setup>
  import PersonComponent from './components/PersonComponent.vue'
 import {ref} from 'vue';

 const person = ref({
     name:"nazmul hossain",
     email:"hossiainnazmul191@gmail.com",
 })
 </script>

<template>
      <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          Original Name: {{ person.name }}<br/>
          Original email: {{ person.email }}<br/>
        </div>

        <div class="mt-10">
          <label>Name</label>
          <p>
            <input type="text" v-model="person.name" /><br><br>
            <input type="text" v-model="person.email" />
          </p>
        </div>
        <br><br>
        <div class="mt-10">
          <label>Component</label><br />
          <PersonComponent label="Name"  :person="person"/>
        </div>
      </div>
</template>

<style scoped>

</style>
