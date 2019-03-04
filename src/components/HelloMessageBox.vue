<template>
  <div class="hello-msg-box">
    <b-card header-tag="header">
      <h6 slot="header" class="mb-0">Message Box Example</h6>
      <b-card-text class="hello-msg-box-card">
        <p>
          {{ message }}
        </p>
        <input v-model="message" />
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: "HelloMessageBox",
  el: "hello-message-box",
  data() {
    return {
      message: ""
    };
  }
};
</script>
