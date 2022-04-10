<script>
  import Title from "$lib/title.svelte";
  import ThemeButton from "$lib/ThemeButton.svelte";
  import "../global/styles.css";
</script>

<header>
  <Title title="Ninja Gaming Guide" />
</header>
<div class="subheader">
  <ThemeButton>Toggle body class</ThemeButton>
</div>

<main>
  <!-- Page content -->
  <slot />
</main>

<footer>
  <p>Copyright 2022 Ninja gaming guides</p>
</footer>

<style lang="scss">
  header {
    display: flex;
    justify-content: center;
  }
  main {
    max-width: 960px;
    margin: 20px auto;
  }
  footer {
    margin-top: auto;
    text-align: center;
    padding-top: 20px;
    padding-bottom: 20px;
  }
  footer p {
    margin: 0;
  }
  .buttonWrapper {
    display: flex;
  }
</style>
