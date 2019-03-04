<template>
  <div id="hello-click">
    <b-card header-tag="header">
      <h6 slot="header" class="mb-0">On Click Example</h6>
      <b-card-text class="hello-msg-box-card">
        <p>{{ message }}</p>
        <button v-on:click="reverseMessage">Reverse Message</button>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "HelloClick",
  el: "hello-click",
  data() {
    return {
      message: "Hello Vue.js!"
    };
  },
  methods: {
    reverseMessage: function() {
      this.message = this.message.split("").reverse().join("") // prettier-ignore
    }
  }
};
</script>
