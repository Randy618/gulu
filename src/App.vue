<template>
  <div id="app">
    <code>
    button color:white,default,primary,success,info,blue,warning,danger,dark
    </code>
    <m-button type="white" embossed rounded transparent >white</m-button>
    <m-button type="default" size="sm">default</m-button>
    <m-button type="primary">primary</m-button>
    <m-button type="success" size="lg">success</m-button>
    <m-button type="info" size="hg">info</m-button>
    <m-button type="blue">blue</m-button>
    <m-button type="warning">warning</m-button>
    <m-button type="danger">danger</m-button>
    <m-button type="dark">dark</m-button>
  </div>
</template>

<script>
import MButton from "./components/button/Button";

export default {
  name: "app",
  components: {
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
