<template>
  <div>
    <h2>标题</h2>
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
h2{
color:red;
}
</style>
