<template>
  <div>
    <h3>Babylon Examples</h3>
    <canvas></canvas>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { PBR } from "@/BabylonExamples/PBR";

export default defineComponent({
  name: 'PBR',
  mounted() {
    const canvas: HTMLCanvasElement = document.querySelector("canvas") as HTMLCanvasElement;
    new PBR(canvas);
    }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

canvas {
  width: 70%;
  height: 70%;
}
</style>
