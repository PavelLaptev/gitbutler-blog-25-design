<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";
  import ThreeArticleRow from "$lib/ThreeArticleRow.svelte";
  import ArticlesList from "$lib/home/ArticlesList.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<div class="content-wrap">
  <Navbar />

  <div class="tag-header">
    <p class="tag-header__query">#TagName</p>
    <p class="tag-header__count">3 posts</p>
  </div>

  <ThreeArticleRow />
  <ThreeArticleRow />
  <ArticlesList />
  <ThreeArticleRow />
  <Footer />
</div>
