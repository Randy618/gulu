<template>
  <div id="app">
    <!--<ui-button></ui-button>-->
    <ui-components></ui-components>
  </div>
</template>

<script>
import uiButton from "./view/ui-button";
import uiComponents from './view/ui-components'

export default {
  name: "app",
  components: {
      uiButton,
      uiComponents
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
