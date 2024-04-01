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
    width: 100%;
    aspect-ratio: 1 / 1;
    border-radius: 16px;
    overflow: hidden;
  }
</style>