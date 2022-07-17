<template>
  <h1>Welcome</h1>
  This page is:
  <ul>
    <li>Rendered to HTML.</li>
    <li>Interactive. <Counter /></li>
    <li v-for="item in todoList" :key="item.id">
    <a :href="`/todos/${item.id}`">
      {{ item.text }}
    </a>
    </li>
  </ul>
</template>

<script lang="ts" setup>
import Counter from './Counter.vue'

const todoList = [
  {
    id: 0,
    text: 'Buy milk',
  },
  {
    id: 1,
    text: 'Buy chocolate',
  },
  {
    id: 2,
    text: 'Buy Chicken',
  },
  {
    id: 3,
    text: 'Buy Drinks',
  },
]
</script>
