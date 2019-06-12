<template>

  <div id="app">
    This is the message to display: {{msg}}

    <welcome></welcome>
  <task-list></task-list>

  </div>

</template>

<script>
 import welcome from "./welcome"
 import newTask from "./newTask"
 import taskList from "./taskList"

export default {
  name: 'app',
  components: {taskList, newTask, welcome},
  data () {
    return {
      msg: 'Lion King'
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
