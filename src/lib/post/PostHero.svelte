<script lang="ts">
  import Navbar from "../Navbar.svelte";
</script>

<div class="post-hero" style="--post-color: rgba(198, 140, 255, 0.20);">
  <div class="content-wrap">
    <Navbar />
    <div class="post-hero__content grid-layout">
      <div class="post-hero__about">
        <div class="post-hero__meta">
          <div class="post-hero__meta-details">
            <p>
              2 days ago by <a href="./author/scott/">Scott Chacon</a>
            </p>
            <p>
              <svg
                width="16"
                height="16"
                viewBox="0 0 16 16"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle
                  cx="8"
                  cy="8.5"
                  r="6.25"
                  stroke="currentColor"
                  stroke-width="1.5"
                />
                <path
                  d="M8 1.5C9.22876 1.5 10.4359 1.82344 11.5 2.43782C12.5641 3.0522 13.4478 3.93587 14.0622 5C14.6766 6.06413 15 7.27124 15 8.5C15 9.72876 14.6766 10.9359 14.0622 12L8 8.5V1.5Z"
                  fill="#1A1614"
                />
              </svg>
              <span>9 min <span class="hide-on-tablet">read</span></span>
            </p>
          </div>

          <div class="post-hero__tags">
            <a class="article__tag-item" href="/tag/git">Git</a>
            <a class="article__tag-item" href="/tag/gitlab">GitLab</a>
            <a class="article__tag-item" href="/tag/cli">CLI</a>
          </div>
        </div>

        <h1 class="post-hero__title">
          How to do patch-based review with git range-diff
        </h1>
        <p class="post-hero__excerpt">
          Diving into `range-diff`, the little known Git power tool to compare
          two versions of a series of patches.
        </p>
      </div>

      <div class="post-hero__image">
        <img
          src="https://blog.gitbutler.com/content/images/size/w800/2025/03/bundle-uri.webp"
          alt="post-preview"
        />
      </div>
    </div>
  </div>
</div>
