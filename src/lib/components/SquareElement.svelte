<!-- TextSquare.svelte -->
<script>
  export let text = 'Default text';
</script>

<div class="text-container">{text}</div>

<style>
  .text-container {
    width: 100%;
    aspect-ratio: 1 / 1;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 16px;
    overflow: hidden;
    background-color: #f0f0f0;
  }
</style>
