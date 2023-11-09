<script setup>
  import TextComponent from './components/TextComponent.vue'
 import {ref} from 'vue';
 const name  = ref('nazmul hossian');
 const email = ref('hossainnazmul191@gmail.com');
 </script>

<template>
      <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          Original Name: {{ name }}<br/>
          Original email: {{ email }}<br/>
        </div>

        <div class="mt-10">
          <label>Name</label>
          <p>
            <input type="text" v-model="name" /><br><br>
            <input type="text" v-model="email" />
          </p>
        </div>
        <br><br>
        <div class="mt-10">
          <label>Component</label><br />
          <TextComponent label="Name" v-model="name"/>
          <TextComponent label="Email" v-model="email"/>
        </div>
      </div>
</template>

<style scoped>

</style>
