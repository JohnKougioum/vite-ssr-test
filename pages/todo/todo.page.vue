<template>
  <h1>To-do</h1>
  <span>{{ todoId }}</span>
  <br />
  <a href="/">Back</a>
</template>

<script setup>
import { usePageContext } from '../../renderer/usePageContext'

const pageContext = usePageContext()
const todoId = parseInt(pageContext.routeParams.todoId)

</script>