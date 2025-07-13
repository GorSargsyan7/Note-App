<template>
  <button class="add-btn">
    +
  </button>
</template>

<script setup>

</script>

<style scoped>
.add-btn{
    position: absolute;
    bottom: 100px;
    right: 100px;
    width: 68px;
    height: 68px;
    border: 2px solid white;
    border-radius: 34px;
    font-size: 35px;
    background: #4CCB90;
    color: #fff;
    cursor: pointer;
    transition: 0.5s;
}
.add-btn:hover{
    background: #38976b;
    transform: scale(1.2);
}

</style>