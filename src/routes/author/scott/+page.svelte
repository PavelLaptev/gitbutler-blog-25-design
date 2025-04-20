<script lang="ts">
  import Navbar from "$lib/Navbar.svelte";
  import ThreeArticleRow from "$lib/ThreeArticleRow.svelte";
  import ArticlesList from "$lib/home/ArticlesList.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<div class="content-wrap">
  <Navbar />

  <div class="bio-large">
    <img
      class="bio-large__avatar"
      src="https://avatars.githubusercontent.com/u/70?v=4"
      alt="Scott Chacon"
    />
    <h1 class="bio-large__title">Written by Scott Chacon</h1>
    <p class="bio-large__about">
      Scott Chacon is a co-founder of GitHub and the founder of GitButler, where
      he builds innovative tools for modern version control. Passionate about
      open source and developer experience, he has authored Pro Git and spoken
      globally on Git and software collaboration.
    </p>
    <div class="bio-large__links">
      <a href="#website">Website</a>
      <a href="#bluesky">Bluesky</a>
      <a href="#x">X</a>
    </div>
  </div>

  <ThreeArticleRow />
  <ThreeArticleRow />
  <ArticlesList />
  <ThreeArticleRow />
  <Footer />
</div>
