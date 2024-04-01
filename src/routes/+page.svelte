<script>
  import SquareElement from '$lib/components/SquareElement.svelte';
  import App from '$lib/components/App.svelte'
</script>

<div class="grid-container">
  <App />
  <SquareElement text="Привет мир" />
  <SquareElement text="Как дела" />
</div>

<style>
  :global(body) {
    background-color: black;
    margin: 0;
    padding: 0; /* Ensures text is visible on the black background */
  }

  .grid-container {
    display: grid;
    gap: 16px;
    padding: 16px;
    grid-template-columns: 1fr; /* Defaults to single-column layout */
  }

  @media (min-width: 768px) { /* Adjusts for wider screens */
    .grid-container {
      grid-template-columns: repeat(2, 1fr); /* Two columns on wider screens */
    }
  }
</style>


<!-- <script>
  import App from '$lib/components/App.svelte'
</script>

<div>
  <App />
</div>

<style>
  :global(body) {
    margin: 0;
  }

  div {
    width: 100vw;
    height: 100vh;
    background: rgb(13, 19, 32);
    background: linear-gradient(180deg, rgba(13, 19, 32, 1) 0%, rgba(8, 12, 21, 1) 100%);
  }
</style> -->
