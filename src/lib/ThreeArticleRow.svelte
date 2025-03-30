<script lang="ts">
  import ThreeColumnBanner from "./baners/threeColumnBanner.svelte";

  interface Props {
    hasBanner?: boolean;
  }

  const { hasBanner = false }: Props = $props();
</script>

<section class="three-post-row">
  <a class="post-card post-card--tablet-hor" href="/how-devs-config-git-core">
    <img
      class="post-card__image"
      alt=""
      src="https://blog.gitbutler.com/content/images/size/w800/2025/01/git_vs_formula_one.webp"
    />
    <div class="post-card__content">
      <h2 class="post-card__title">
        Why is Git Autocorrect too fast for Formula One drivers?
      </h2>
      <p class="post-card__caption">
        5 days ago by Scott Chacon — <i>9 min read</i>
      </p>
      <p class="post-card__excerpt">
        Why does Git's autocorrect wait 0.1s before executing a mistyped
        command? Let's dig in.
      </p>
    </div>
  </a>

  <a class="post-card post-card--tablet-hor" href="/how-devs-config-git-core">
    <img
      class="post-card__image"
      alt=""
      src="https://blog.gitbutler.com/content/images/size/w800/2024/12/stacking.jpg"
    />
    <div class="post-card__content">
      <h2 class="post-card__title">Stacked Branches with GitButler</h2>
      <p class="post-card__caption">
        5 days ago by Scott Chacon — <i>9 min read</i>
      </p>
      <p class="post-card__excerpt">
        GitButler can now manage dependent branches that are stacked, including
        managing stacked GitHub PRs.
      </p>
    </div>
  </a>

  {#if hasBanner}
    <ThreeColumnBanner />
  {:else}
    <a class="post-card post-card--tablet-hor" href="/how-devs-config-git-core">
      <img
        class="post-card__image"
        alt=""
        src="https://blog.gitbutler.com/content/images/size/w800/2024/10/git-merge-email-2.png"
      />
      <div class="post-card__content">
        <h2 class="post-card__title">Git Merge 2024 Talks are Up</h2>
        <p class="post-card__caption">
          5 days ago by Scott Chacon — <i>9 min read</i>
        </p>
        <p class="post-card__excerpt">
          All the Git Merge 2024 talks are up on Youtube. Here is a quick
          summary of each one.
        </p>
      </div>
    </a>
  {/if}
</section>
