<script>
  function toggleBodyClassname() {
    window.document.body.classList.toggle("dark-mode");
  }
  export let buttontitle = "button";
</script>

<button on:click={toggleBodyClassname} title={buttontitle}>
  <slot />
</button>

<style>
  button {
    padding: 20px;
    border-radius: 10px;
    border: none;
    text-transform: uppercase;
  }
  :global(body.dark-mode) button {
    background-color: red;
    color: white;
  }
</style>
