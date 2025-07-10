<template>
<RouterView/>
<div v-for="pix in arr">
<PixCounter  v-if="pix.age <= 10" :name="pix.name" :age="pix.age" :count="pix.count"/>
</div>
</template>

<script setup>
import { RouterView } from 'vue-router'
import PixCounter from './components/PixCounter.vue'
import { ref } from 'vue';

let arr = ref([
  {
    name:'Luna',
    age: 5,
    count: 1
  },
    {
    name:'Ronaldo',
    age: 40,
    count: 1
  },
    {
    name:'Aaaa',
    age: 59,
    count: 2
  },
])
</script>

<style>

</style>
