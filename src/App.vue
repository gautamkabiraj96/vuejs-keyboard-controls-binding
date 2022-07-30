<template>
  <div id="app">
    <button @click.ctrl="onClick">Ctrl + Click me</button>
    <button @click.alt="onClick">Alt + Click me</button>
    <button @click.ctrl.exact="onClick">Ctrl exact + Click me</button>
    <button @click.left="onClick">Left mouse button</button>
    <button @click.right="onClick">Right mouse button</button>
    <button @click.middle="onClick">Middle mouse button</button>
    <div class="np-credits">wwww.nightprogrammer.com</div>
  </div>
</template>

<script>
export default {
  name: "App",
  methods: {
    onClick() {
      alert("Clicked!");
    },
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 24px;
}

button {
  margin-top: 0.5em;
  background-color: #004cbe;
  color: #ffffff;
  border: 0px;
  border-radius: 6px;
  padding: 6px 20px;
  margin-right: 1em;
  cursor: pointer;
  transition: all 0.3s;
}

button:hover {
  background-color: #2f79e7;
  transition: all 0.3s;
}

.np-credits {
  font-size: 12px;
  margin-top: 12px;
  color: #4b4b4b;
}
</style>