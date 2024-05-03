<template>
    <div>
      <h2>Contador: {{ count }}</h2>
      <button> @click="decrement">-</button>
      <button> @click="increment">+</button>
    </div>
  </template>
  
  <style scoped>
  button {
    margin: 5px;
    padding: 5px;
  }
  </style>
  
  <script>
  export default {
    data() {
      return {
        count: 0
      };
    },
    methods: {
      increment() {
        this.count++;
      },
      decrement() {
        this.count--;
      }
    }
  };
  </script>