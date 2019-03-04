<template>
  <div id="app" class="container">
    <div class="example">
      <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
      <Hello name="Timmmy" age="29" />
      <HelloList />
      <HelloClick />
      <HelloMessageBox />
    </div>
    <!-- <HelloWorld msg="A different message" /> -->
  </div>
</template>

<script>
import Hello from "./components/Hello.vue";
import HelloList from "./components/HelloList.vue";
import HelloClick from "./components/HelloClick.vue";
import HelloMessageBox from "./components/HelloMessageBox.vue";

export default {
  name: "app",
  components: {
    Hello,
    HelloList,
    HelloClick,
    HelloMessageBox
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.container {
  display: flex;
  justify-content: center;
}
.example {
  display: flex;
  justify-content: space-around;
  width: 800px;
  margin: 50px 0;
}
</style>
