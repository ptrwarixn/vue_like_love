<template>
  <div id="app">
    <div class="row">
      <div class="col-6">
        <img src="./assets/1_1edit.jpg" style="width=50px" />
        <emobutton />
      </div>
      <div class="col-6">
        <img src="./assets/1_2edit.jpg" alt=" " />
        <emobutton />
      </div>
    </div>
    <div class="row">
      <div class="col-6">
        <img src="./assets/2_1edit.jpg" style="width=50px" />
        <emobutton />
      </div>
      <div class="col-6">
        <img src="./assets/2_2edit.jpg" alt=" " />
        <emobutton />
      </div>
    </div>
    <div class="row">
      <div class="col-6">
        <img src="./assets/3_1edit.jpg" style="width=50px" />
        <emobutton />
      </div>
      <div class="col-6">
        <img src="./assets/3_2edit.jpg" alt=" " />
        <emobutton />
      </div>
    </div>
  </div>
</template>

<script>
import emobutton from "./components/emobutton.vue";

export default {
  name: "App",
  components: {
    emobutton,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(88, 0, 88);
  margin-top: 60px;
  background-color: rgb(255, 255, 255);
}
</style>
