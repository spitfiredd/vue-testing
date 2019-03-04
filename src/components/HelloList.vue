<template>
  <div class="hello-list">
    <b-card header-tag="header">
      <h6 slot="header" class="mb-0">List Example</h6>
      <b-card-text class="hello-list-card">
        <ol class="hello-list-list-style">
          <li v-for="todo in todos" v-bind:key="todo">{{ todo.text }}</li>
        </ol>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "HelloList",
  el: "hello-list",
  data() {
    return {
      todos: [
        { text: "Learn JavaScript" },
        { text: "Learn Vue" },
        { text: "Build something awesome" }
      ]
    };
  }
};
</script>

<style scoped>
.hello-list-card {
  text-align: left;
}
.hello-list-list-style {
  font-size: 11px;
}
</style>
