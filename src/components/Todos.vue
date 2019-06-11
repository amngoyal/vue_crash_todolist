<template>
  <div>
    <div v-bind:key="todo" v-for="todo in todos">
      <Todoitem v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>
export default {
  name: "Todos",
  components: {
    Todoitem
  },
  props: ["todos"]
};
</script>

<style scoped>
</style>
