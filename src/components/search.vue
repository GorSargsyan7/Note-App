<template>
    <form class="input-box" role="search">
        <input v-model="search" placeholder="Search note" />
        <button type="button" @click="$emit('onSearch',search)">Search</button>
    </form>
</template>

<script setup>
import { ref } from 'vue';

const search =ref('')
</script>

<style>
.input-box {
    display: flex;
    height: 40px;
    max-width: 400px;
    width: 100%;
    gap: 6px;
}

.input-box input {
    width: 100%;
    padding-left: 30px;
}

.input-box button {
    background-color: rgb(0, 161, 0);
    color: white;
    border-radius: 5px;
    border: 1px solid #fff;
}
</style>