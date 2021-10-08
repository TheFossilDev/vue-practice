<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from './Button'

export default {
  name: "Header",
  // Just importing an array of prop pointers to look for
  // props: ['title'],

  props: {
    // Define type
    // title: String,
    title: {
      type: String,
      default: 'Hello World'
    },
  },
  components: {
    // List imported components?
    Button,
  }
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
