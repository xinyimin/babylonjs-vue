<template>
  <div>
    <h1>babylonjs项目</h1>

    <canvas class="bjsCanvas" ref="bjsCanvas" />
  </div>
</template>

<script>
import { createScene } from "../scenes/MyFirstScene";

export default {
  name: "BabylonScene",

  mounted() {
    const bjsCanvas = this.$refs.bjsCanvas;
    if (bjsCanvas) {
      createScene(bjsCanvas);
    }
  },
};
</script>
<style scoped>
.bjsCanvas {
  width: 80vw;
  height: 80vh;
  background-color: rgb(173, 34, 34);
}
h1 {
  color: rgb(173, 34, 34);
}
</style>

