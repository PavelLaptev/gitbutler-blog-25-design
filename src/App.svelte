<script lang="ts">
  import Home from "./Home.svelte";
  import Article from "./Article.svelte";

  let isURLArticle = $state(false);

  $effect(() => {
    console.log("URL changed");
    const url = new URL(window.location.href);
    const path = url.pathname;
    isURLArticle = path.startsWith("/article");
  });
</script>

<main class="page">
  {#if isURLArticle}
    <Article />
  {:else}
    <Home />
  {/if}
</main>
