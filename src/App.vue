<script setup>
    import ComponentA from './components/ComponentA.vue';
    import {person} from './store/data.js';

 </script>

<template>
      <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Model</h1>
        </div>

        <div class="mt-10">
          Original Name: {{ person.name }}<br/>
        </div>

        <div class="mt-10">
            <ComponentA />
        </div>

      </div>
</template>

<style scoped>

</style>
