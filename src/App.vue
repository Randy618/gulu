<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <code>
    button color:white,default,primary,success,info,blue,warning,danger,dark
    </code>
    <m-button color="white" embossed rounded transparent >white</m-button>
    <m-button color="default">default</m-button>
    <m-button color="primary">primary</m-button>
    <m-button color="success">primary</m-button>
    <m-button color="info">info</m-button>
    <m-button color="blue">blue</m-button>
    <m-button color="warning">warning</m-button>
    <m-button color="danger">danger</m-button>
    <m-button color="dark">dark</m-button>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import MButton from "./components/button/Button.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
      MButton
  }
};
</script>

<style lang="less">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
