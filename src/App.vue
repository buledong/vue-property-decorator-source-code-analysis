<template>
  <div id="app">
    <HelloWorld />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

// 用法一, 直接装饰类, 没有传入参数
import { Component, Vue } from "vue-property-decorator";
@Component({
  name: "App",
  components: {
    HelloWorld,
  },
})
class App extends Vue {}
export default App;
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
