<script>
  import Navbar from "./lib/Navbar.svelte";
  import Hero from "./lib/home/Hero.svelte";
  import FeaturedArticles from "./lib/home/FeaturedArticles.svelte";
  import YTPromo from "./lib/home/YTPromo.svelte";
  import ThreeArticleRow from "./lib/ThreeArticleRow.svelte";
  import Subscribe from "./lib/Subscribe.svelte";
  import ArticlesList from "./lib/home/ArticlesList.svelte";
</script>

<main class="page">
  <div class="page-content">
    <Navbar />
    <Hero />
    <FeaturedArticles />
    <YTPromo />
    <ThreeArticleRow />
    <Subscribe />
    <ThreeArticleRow />
    <ArticlesList />
    <ThreeArticleRow hasBanner />
  </div>
</main>
