<template>
  <div id="app">
    <Player/>
  </div>
</template>

<script>
import Player from './components/Player.vue';

export default {
  name: 'App',
  components: {
    Player,
  },
};
</script>

<style>
#app {
  font-family: "Rambla", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: red url("./assets/bg.jpg") no-repeat center center;
  width: 800px;
  height: 600px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
