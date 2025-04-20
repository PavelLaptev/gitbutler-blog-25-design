<script lang="ts">
  import "../styles/main.css";
  let { children } = $props();
</script>

<main class="page">
  {@render children()}
</main>
