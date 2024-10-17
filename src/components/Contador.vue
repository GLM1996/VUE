<template>
    <h1>Hola</h1>
    <button @click="incrementar">
      Incrementar
    </button>
    <button @click="decrementar">
      Decrementar
    </button>
    <p>{{ count }}</p>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const count = ref(0)
  
  const incrementar = () =>{
    count.value++
  }
  const decrementar = () =>{
    count.value--
  }
  
  </script>
  
  <style scoped>
    button{
      background-color: blue;
      color: white;
      margin-left: 10px;
      cursor: pointer;
    }
  </style>
  