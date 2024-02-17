<script setup>
import { ref, reactive } from 'vue'

import PersonComponent from "./components/PersonComponent.vue";

const person = reactive({
  name: 'John Doe',
  email: 'john@doe.xom'
})
</script>

<template>
  <h3>Component Model Class Practice</h3>
  <section class="mx-auto mt-5 bg-red-400">
    <label for="" class="text-3xl ">Parent Component</label>
    <p>Name: {{ person.name }}<br>
      <input class="mx-auto p-5 m-5 text-xl" type="text" v-model="person.name"><br>
      Email: {{ person.email }}<br>
      <input class="mx-auto  p-5 m-5 text-xl" type="text" v-model="person.email"><br>
    </p>
  </section>
  <section class="mx-auto mt-5 bg-blue-500 p-5 m-5 text-white font-bold ">
    <PersonComponent :person="person" />
  </section>
</template>

<style scoped></style>
