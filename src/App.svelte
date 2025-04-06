<script lang="ts">
  import Home from "./Home.svelte";
  import Post from "./Post.svelte";

  let isURLArticle = $state(false);

  $effect(() => {
    console.log("URL changed");
    const url = new URL(window.location.href);
    const path = url.pathname;
    isURLArticle = path.startsWith("/post");
  });
</script>

<main class="page">
  {#if isURLArticle}
    <Post />
  {:else}
    <Home />
  {/if}
</main>
