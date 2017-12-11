<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <span v-if="nameIsShow">{{name}}</span>
    <ul>
      <li v-for="todo in todos">
        {{todo.text}}
      </li>
    </ul>
    <input v-model="message">
    <span>{{message}}</span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      message: '',
      msg: 'vue 练习',
      name: 'yanmeng',
      nameIsShow: false,
      todos: [{
        text: '1'
      }, {
        text: '2'
      }]
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
