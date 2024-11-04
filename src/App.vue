<script setup>
import { ref, reactive, computed, watch } from 'vue'
const names = reactive(['Gruber, Hans', 'Bellic, Niko', 'Commando, Captain'])
const selected = ref('')
const prefix = ref('')
const first = ref('')
const last = ref('')




</script>

<template>
  <div><input v-model="prefix" placeholder="Filter prefix"></div>



  <label>Name: <input v-model="first"></label>
  <label>Surname: <input v-model="last"></label>

  <div class="buttons">
    <button @click="create">Create</button>
    <button @click="update">Update</button>
    <button @click="del">Delete</button>
  </div>
</template>

<style>
* {
  font-size: inherit;
}







</style>
