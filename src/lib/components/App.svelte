<script>
  import { Canvas } from '@threlte/core';
  import Scene from './Scene.svelte';
</script>

<div class="scene-container">
  <Canvas>
    <Scene />
  </Canvas>
</div>

<style>
  .scene-container {
    background: radial-gradient(circle at 50% 50%, #383691, #333 100%);
    width: 100%;
    aspect-ratio: 1 / 1;
    border-radius: 16px;
    overflow: hidden;
  }
</style>