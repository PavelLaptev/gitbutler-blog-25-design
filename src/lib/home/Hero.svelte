<article class="hero">
  <img
    class="hero-image"
    alt=""
    src="https://blog.gitbutler.com/content/images/size/w800/2025/03/bundle-uri.webp"
  />

  <div class="hero-content">
    <p class="hero-caption">
      5 days ago by Scott Chacon — <i>9 min read</i>
    </p>
    <h2 class="hero-title">How to do patch-based review with git range-diff</h2>
    <p class="hero-excerpt">
      Diving into `range-diff`, the little known Git power tool to compare two
      versions of a series of patches.
    </p>
    <!-- there is a special css that truncates the text up to 4 lines -->
    <p class="hero-description">
      This all started with me trying to figure out the state of a feature that
      I had heard about from GitLab's Gitaly project called bundle-uri, which
      allows you to, in theory, speed up a clone by downloading a cached file
      that seeds your project's data before doing a server CPU-intensive fetch.
      In a nutshell, when you clone a Git repository, the git clone command will
      start a conversation with the Git server you're connecting to in order to
      figure out what all is available on the server and what it would like to
      get.
    </p>
  </div>
</article>
