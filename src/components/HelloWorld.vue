<template>
  <div>
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
  width: 100vw;
  height: 100vh;
}
</style>