<template>
  <div id="app">
    <!-- <HelloWorld v-bind:cities="cities" /> -->
    <Header v-bind:title="pageTitle" />
    <AddTodo />
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/layouts/Header";
import Todos from "./components/layouts/Todos";
import AddTodo from "./components/layouts/AddTodo";

export default {
  name: "App",
  components: {
    // HelloWorld,
    Header,
    Todos,
    AddTodo,
  },
  data() {
    return {
      // cities: ["서울", "부산", "대구", "대전", "군산", "울산", "광주"],
      pageTitle: "Todo 앱",
      todos: [
        { id: 1, title: "dentist", complete: true },
        { id: 2, title: "study", complete: false },
        { id: 3, title: "dinner", complete: true },
        { id: 4, title: "sleep", complete: true },
        { id: 5, title: "sleep", complete: false },
        { id: 6, title: "sleep", complete: false },
      ],
    };
  },
  methods: {
    addtodo() {
      console.log(AddTodo.);
    },
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
</style>
