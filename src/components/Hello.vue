<template>
  <div class="world">
    <b-card header-tag="header">
      <h6 slot="header" class="mb-0">Hello Example</h6>
      <b-card-text class="hello-card">
        <h8><strong>Hello:</strong> {{ name }}</h8> <br />
        <h8><strong>You are:</strong> {{ age }}</h8>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "Hello",
  el: "world",
  props: {
    name: String,
    age: Number
  }
};
</script>

<style scoped>
.hello-card {
  text-align: left;
}
</style>
