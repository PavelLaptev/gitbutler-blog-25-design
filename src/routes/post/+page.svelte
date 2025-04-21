<script lang="ts">
  import PostHero from "$lib/post/PostHero.svelte";
  import PostsCarousel from "$lib/post/PostsCarousel.svelte";
  import Subscribe from "$lib/Subscribe.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<PostHero />

<div class="post-content">
  <div class="grid-layout">
    <div class="post-share-links">
      <a
        class="post-share-btn hackernews"
        href="#link"
        aria-label="Share on Hacker News"
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M5 1C2.79086 1 1 2.79086 1 5V19C1 21.2091 2.79086 23 5 23H19C21.2091 23 23 21.2091 23 19V5C23 2.79086 21.2091 1 19 1H5ZM7.9957 4.64648H6L11.2001 13.4648V19.6465H12.9428V13.4648L18.1429 4.64648H16.1472L12.1558 11.6484H11.9871L7.9957 4.64648Z"
            fill="currentColor"
          />
        </svg>
      </a>
      <a class="post-share-btn blsk" href="#link" aria-label="Share on BlueSky">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M5.76879 4.27893C8.29104 6.13626 11.004 9.90214 12.0001 11.9231C12.9962 9.90228 15.709 6.13622 18.2313 4.27893C20.0513 2.93876 23 1.90182 23 5.20144C23 5.86042 22.6148 10.7372 22.3889 11.5289C21.6036 14.2815 18.7421 14.9836 16.1967 14.5587C20.646 15.3014 21.7778 17.7617 19.3335 20.2221C14.6911 24.8947 12.661 19.0497 12.1406 17.552C12.0453 17.2774 12.0007 17.149 12 17.2582C11.9993 17.149 11.9547 17.2774 11.8594 17.552C11.3392 19.0497 9.30916 24.8948 4.66654 20.2221C2.22213 17.7617 3.35395 15.3013 7.80331 14.5587C5.25785 14.9836 2.39627 14.2815 1.6111 11.5289C1.38518 10.7371 1 5.86034 1 5.20144C1 1.90182 3.94882 2.93876 5.76866 4.27893H5.76879Z"
            fill="currentColor"
          />
        </svg>
      </a>
      <a
        class="post-share-btn linkedin"
        href="#link"
        aria-label="Share on LinkedIn"
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M20.381 1H3.61905C2.17333 1 1 2.17333 1 3.61905V20.381C1 21.8267 2.17333 23 3.61905 23H20.381C21.8267 23 23 21.8267 23 20.381V3.61905C23 2.17333 21.8267 1 20.381 1ZM7.80952 9.38095V19.3333H4.66667V9.38095H7.80952ZM4.66667 6.48429C4.66667 5.75095 5.29524 5.19048 6.2381 5.19048C7.18095 5.19048 7.77286 5.75095 7.80952 6.48429C7.80952 7.21762 7.22286 7.80952 6.2381 7.80952C5.29524 7.80952 4.66667 7.21762 4.66667 6.48429ZM19.3333 19.3333H16.1905C16.1905 19.3333 16.1905 14.4829 16.1905 14.0952C16.1905 13.0476 15.6667 12 14.3571 11.979H14.3152C13.0476 11.979 12.5238 13.0581 12.5238 14.0952C12.5238 14.5719 12.5238 19.3333 12.5238 19.3333H9.38095V9.38095H12.5238V10.7219C12.5238 10.7219 13.5348 9.38095 15.5671 9.38095C17.6467 9.38095 19.3333 10.811 19.3333 13.7076V19.3333Z"
            fill="currentColor"
          />
        </svg>
      </a>
      <a class="post-share-btn x" href="#link" aria-label="Share on X">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M18.0113 3.32812H20.9237L14.5292 10.6873L22 20.6702H16.1373L11.5472 14.6037L6.29224 20.6702H3.37987L10.1543 12.7991L3 3.32812H9.00833L13.1553 8.8699L18.0113 3.32812ZM16.992 18.9424H18.6065L8.15995 4.99194H6.42519L16.992 18.9424Z"
            fill="currentColor"
          />
        </svg>
      </a>
      <button class="post-share-btn copy-link" aria-label="Copy link">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M3.96962 13.0303C1.60566 10.6664 1.60567 6.83365 3.96963 4.46969C6.33359 2.10573 10.1663 2.10573 12.5303 4.46969L14.4053 6.34469L13.3446 7.40535L11.4696 5.53035C9.69145 3.75217 6.80846 3.75217 5.03029 5.53035C3.25211 7.30852 3.25211 10.1915 5.03028 11.9697L6.90529 13.8447L5.84463 14.9053L3.96962 13.0303ZM20.0303 11.9697C22.3943 14.3337 22.3942 18.1664 20.0303 20.5303C17.6663 22.8943 13.8336 22.8943 11.4696 20.5303L9.59463 18.6553L10.6553 17.5947L12.5303 19.4697C14.3085 21.2479 17.1915 21.2479 18.9696 19.4697C20.7478 17.6915 20.7478 14.8085 18.9696 13.0303L17.0946 11.1553L18.1553 10.0947L20.0303 11.9697ZM15.863 15.3024L9.1963 8.6357L8.13564 9.69636L14.8023 16.363L15.863 15.3024Z"
            fill="currentColor"
          />
        </svg>
      </button>
    </div>

    <section class="post-content__body">
      <div class="off-grid-wrapper">
        <div class="post__table-of-contents off-grid-container">
          <h3>Table <i>of</i> Contents</h3>
          <ul>
            <li>
              <a class="selected" href="#section-1"
                >Finding the diff between two branch versions</a
              >
            </li>
            <li>
              <a href="#section-2">What Changed?</a>
            </li>
            <li>
              <a href="#section-3">A Simple Example</a>
            </li>
            <li>
              <a href="#section-4">Range Diff</a>
            </li>
            <li>
              <a href="#section-5">Diff of Diffs</a>
            </li>
            <li>
              <a href="#section-6">Patch Order</a>
            </li>
            <li>
              <a href="#section-7">Metadata</a>
            </li>
          </ul>
        </div>
      </div>

      <p>
        A few weeks ago I wrote about Git’s help.autocorrect setting and the
        strange tale of the origin of it’s deciseconds value.
      </p>
      <p>
        It got me to thinking about other git config settings that most people
        likely don’t know about and which should probably be defaulted
        differently.
      </p>
      <p>
        In this post, I’ll go through some of the perhaps obscure Git config
        settings that I have personally globally enabled and go into them to
        explain what they do and why they should probably be the default
        settings.
      </p>
      <p>
        Also, it turns out that I learned most of these from the people who
        actually work on the core Git codebase every day.
      </p>

      <pre>
          <code
          >time git clone https://gitlab.com/gitlab-org/gitlab-foss.git g1
Cloning into 'g1'...
  remote: Enumerating objects: 3005985, done.
  remote: Counting objects: 100% (314617/314617), done.
  remote: Compressing objects: 100% (64278/64278), done.
  remote: Total 3005985 (delta 244429), reused 311002 (delta 241404), 
          pack-reused 2691368 (from 1)
  Receiving objects: 100% (3005985/3005985), 1.35 GiB | 23.91 MiB/s
  Resolving deltas: 100% (2361484/2361484), done.
  Updating files: 100% (59972/59972), done.
(*) 162.93s user 37.94s system 128% cpu 2:36.49 total</code
        >
        </pre>

      <div class="off-grid-wrapper">
        <div class="post__hiring-banner off-grid-container">
          <h3 class="post__hiring-banner__title"><i>We’re</i> hiring!</h3>
          <div class="post__hiring-banner__content">
            <a
              class="post__hiring-banner__position"
              href="https:https://app.gitbutler.com"
            >
              <h4 class="post__hiring-banner__position-title">
                Senior TypeScript Developer
              </h4>
              <p class="post__hiring-banner__position-description">
                We're looking for an experienced TypeScript developer to join
                our team in Berlin to help us build the next generation Git
                client.
              </p>
              <p class="post__hiring-banner__position-caption">
                Full-time — BERLIN
              </p>
            </a>
            <a
              class="post__hiring-banner__position"
              href="https:https://app.gitbutler.com"
            >
              <h4 class="post__hiring-banner__position-title">
                Senior TypeScript Developer
              </h4>
              <p class="post__hiring-banner__position-description">
                We're looking for an experienced TypeScript developer to join
                our team in Berlin to help us build the next generation Git
                client.
              </p>
              <p class="post__hiring-banner__position-caption">
                Full-time — BERLIN
              </p>
            </a>
          </div>

          <img
            class="post__hiring-banner__illustration"
            src="/hiring-guy.svg"
            alt=""
          />
        </div>
      </div>

      <p>
        If you interactive rebase, squash, fixup, and otherwise mangle your
        branch and someone wants to know the interdiff - the difference between
        the first version of your branch and a subsequent version, how do you
        find that difference? This is where git range-diff comes into play.
      </p>

      <p>
        Let's try to speed this up by putting all those objects into a packfile,
        using the newer <code>bundle-uri</code> option to
        <code>git clone</code> to pull those from a CDN, then doing what should be
        basically a no-op fetch.
      </p>

      <h2>What is bundle-uri?</h2>

      <p>
        If you're not familiar with bundle files, it's actually an <em
          >incredibly</em
        >
        old command that was introduced in Git 1.5.1 (in 2007 - 18 years ago) called
        <code>git bundle</code>, the purpose of which, as stated in the
        <a
          href="https://github.com/git/git/blob/cb0ae672aeabefca9704477ea8018ac94f523970/Documentation/RelNotes/1.5.1.adoc?ref=blog.gitbutler.com#L66-L67"
          rel="noreferrer">release notes</a
        >, was to make "sneakernetting" easier - putting the repository on a USB
        stick and walking it around the office.
      </p>

      <p>
        Basically it produces a repository in a file - sort of a packfile with a
        list of references as a pre-header. You can <a
          href="https://git-scm.com/book/en/v2/Git-Tools-Bundling?ref=blog.gitbutler.com"
          rel="noreferrer">read all about it</a
        > in my old Pro Git book if you want to dig into them a bit more.
      </p>

      <p>
        So, let's make a repository in a file of the current state of the GitLab
        codebase, which we can do with <code
          >git bundle create [file] --all</code
        >.
      </p>

      <div class="off-grid-wrapper">
        <figure class="off-grid-container">
          <iframe
            class="embed-video"
            src="https://www.youtube.com/embed/B5VQ0L3uL6M?si=-JHCsm_LSBu6tD59"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
            referrerpolicy="strict-origin-when-cross-origin"
            allowfullscreen
          ></iframe>

          <figcaption>
            Here is a video of me doing this in action. I’m using the
            <a
              href="https://gitlab.com/gitlab-org/gitlab-foss/-/tree/4c0f3b8e1d2c5f7a6b9d4e0f1a2b3c4d5e6f7g8h"
              rel="noreferrer">GitLab</a
            >
            repository as an example, but you can use any repository you want.
          </figcaption>
        </figure>
      </div>

      <pre><code
          >❯ time git bundle create gitlab-base.bundle --all
          Enumerating objects: 3005710, done.
          Counting objects: 100% (3005710/3005710), done.
          Delta compression using up to 8 threads
          Compressing objects: 100% (582467/582467), done.
          Writing objects: 100% (3005710/3005710), 1.35 GiB | 194.33 MiB/s, done.
          Total 3005710 (delta 2361291), reused 3005710 (delta 2361291), pack-reused 0 (from 0)
          (*)  17.31s user 3.03s system 84% cpu 24.199 total</code
        ></pre>

      <p>
        If you think about it, the patches and tarballs workflow is sort of the
        first distributed version control system - everyone has a local copy,
        the changes can be made locally, access to "merge" is whomever can push
        a new tarball to the server.
      </p>

      <figure>
        <iframe
          class="embed-video"
          src="https://www.youtube.com/embed/MPFgOnACULU?si=54j-BdXXtGS-82mb"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          referrerpolicy="strict-origin-when-cross-origin"
          allowfullscreen
        ></iframe>

        <figcaption>
          If you want to learn more about Bitkeeper, check out this Bits and
          Booze episode where we set it up and show you how it was used.
        </figcaption>
      </figure>

      <h2 id="the-first-commit">The First Commit</h2>

      <div class="off-grid-wrapper">
        <a
          class="three-col-banner off-grid-container"
          href="https://app.gitbutler.com"
          target="_blank"
        >
          <div
            class="three-col-banner__image-bg"
            style="background-image: url('/new-branch-illustration.svg');"
          ></div>
          <h1 class="three-col-banner__title">
            Boost your Git workflow<br />with GitButler
          </h1>
        </a>
      </div>

      <p>
        Since we're on the topic, what did the <a
          href="https://github.com/git/git/commit/e83c5163316f89bfbde7d9ab23ca2e25604af290?ref=blog.gitbutler.com"
          rel="noreferrer">first commit</a
        > look like? What could Git do from it’s first moment of existence?
      </p>

      <p>
        Well, it was a <strong>stupid content tracker</strong>. As Linus himself
        put it
        <a
          href="https://github.com/git/git/commit/e83c5163316f89bfbde7d9ab23ca2e25604af290?ref=blog.gitbutler.com#diff-2b7814d3fca2e99e56c51b6ff2aa313ea6e9da6424804240aa8ad891fdfe0900R15-R17"
          rel="noreferrer">from day one</a
        >:
      </p>

      <blockquote>
        This is a stupid (but extremely fast) directory content manager. It
        doesn't do a whole lot, but what it <em>does</em> do is track directory contents
        efficiently.
      </blockquote>

      <p>
        The first commit was a collection of seven simple stand alone tools.
        They weren’t things like <code>git commit</code>, they were very low
        level database tools like <code>write-tree</code> and
        <code>commit-tree</code>
        (<a
          href="https://lore.kernel.org/git/Pine.LNX.4.58.0504291416190.18901@ppc970.osdl.org/?ref=blog.gitbutler.com"
          >this changed</a
        >
        a few weeks into the project, when everything started being prefixed with
        <code>git-</code>).
      </p>

      <div class="off-grid-wrapper">
        <div class="post__related-articles off-grid-container">
          <h3>Related <i>articles</i></h3>
          <ul>
            <li>
              <a href="#section-1">How Core Git Developers Configure Git</a>
              <p>by Scott Chacon — <i>13 min read</i></p>
            </li>
            <li>
              <a href="#section-2"
                >Why is Git Autocorrect too fast for Formula One drivers?</a
              >
              <p>by Scott Chacon — <i>8 min read</i></p>
            </li>
            <li>
              <a href="#section-3">Git's Bundle URI</a>
              <p>by Scott Chacon — <i>5 min read</i></p>
            </li>
          </ul>
        </div>
      </div>

      <ul>
        <li>
          Build up a “snapshot” by using <code>update-cache</code> to build a
          cache of contents (essentially a tarball), and
          <code>write-tree</code> to write it as an object to the database.
        </li>
        <li>
          Write a "changeset" (commit) with <code>commit-tree</code> that commented
          on the changes introduced with a new tarball and the parent it was based
          on in order to setup a history of “tarballs”.
        </li>
        <li>
          Read out those database structures with <code>cat-file</code>
          (pull an object out of the database), <code>read-tree</code> (list out
          what the cache looks like) and <code>show-diff</code> (show the diff of
          the cache to the working directory).
        </li>
      </ul>

      <p>
        From the very first days, Linus <a
          href="https://lore.kernel.org/git/Pine.LNX.4.58.0504170916080.7211@ppc970.osdl.org/?ref=blog.gitbutler.com"
          >mentions</a
        > that he really only wanted to build this plumbing and have it be the backend
        for some UI (“porcelain”) be scripted on top of it.
      </p>

      <figure class="kg-card kg-image-card kg-card-hascaption">
        <img
          src="https://blog.gitbutler.com/content/images/2025/04/CleanShot-2025-04-05-at-08.30.42@2x.png"
          alt=""
          loading="lazy"
          width="1914"
          height="1520"
          srcset="https://blog.gitbutler.com/content/images/size/w600/2025/04/CleanShot-2025-04-05-at-08.30.42@2x.png 600w, https://blog.gitbutler.com/content/images/size/w1000/2025/04/CleanShot-2025-04-05-at-08.30.42@2x.png 1000w, https://blog.gitbutler.com/content/images/size/w1600/2025/04/CleanShot-2025-04-05-at-08.30.42@2x.png 1600w, https://blog.gitbutler.com/content/images/2025/04/CleanShot-2025-04-05-at-08.30.42@2x.png 1914w"
          sizes="(min-width: 720px) 720px"
        />
        <figcaption>
          <span
            >The version of git-scm.com that I first put up in 2008. It's a
            "blob" eating "trees".</span
          >
        </figcaption>
      </figure>

      <p>
        However, in this world, the version control systems of the time were
        simply not helpful - they seemed like a step backward in functionality.
        They had clunky access control mechanisms, they weren’t distributed,
        they were incredibly slow.
      </p>

      <p>
        So, Linus decided to build a new version control system that was
        distributed, fast, and had a simple access control mechanism. He wanted
        to be able to do things like <code>git clone</code> and
        <code>git push</code> without having to worry about the underlying implementation.
      </p>

      <h3 id="the-first-git-rebase">The first <code>git rebase</code></h3>

      <p>
        There are lots of these “firsts”, but I’ll just do one more because I
        find it so interesting. The infamous “rebase” command was <a
          href="https://lore.kernel.org/git/Pine.LNX.4.58.0506211452110.2353@ppc970.osdl.org/?ref=blog.gitbutler.com"
          rel="noreferrer">born from a conversation</a
        > about workflow between Junio and Linus in June 2005.
      </p>

      <a href="#link">
        <img
          class="large-image"
          src="https://cdn.glitch.global/d7b566eb-2c6b-489c-a6ea-f4518a2c9fc2/gb-banner.jpg?v=1744550947590"
          alt=""
        /></a
      >

      <p>
        I started using Git for something you might not imagine it was intended
        for, only a few months after it’s first commit. I then went on to
        cofound <a
          href="https://github.com/?ref=blog.gitbutler.com"
          rel="noreferrer">GitHub</a
        >, write arguably the most widely read
        <a href="https://git-scm.com/book/en/v2?ref=blog.gitbutler.com"
          >book on Git</a
        >, build the
        <a
          href="https://lore.kernel.org/git/d411cc4a0807251035i7aed2ec9wef7e8f1b3ae4c585@mail.gmail.com/?ref=blog.gitbutler.com"
          >official website</a
        >
        of the project, start the
        <a
          href="https://github.blog/news-insights/the-library/git-merge-berlin-2013/?ref=blog.gitbutler.com"
          >annual developer conference</a
        >, etc - this little project has changed the world of software
        development, but more personally, it has massively changed the course of
        my life.
      </p>

      <div class="post-bio">
        <img
          class="post-bio__avatar"
          src="https://avatars.githubusercontent.com/u/70?v=4"
          alt="Scott Chacon"
        />
        <div class="post-bio__content">
          <p class="post-bio__title">
            Written by <a href="#all-articles">Scott Chacon</a>
          </p>
          <p class="post-bio__about">
            Scott Chacon is a co-founder of GitHub and the founder of GitButler,
            where he builds innovative tools for modern version control.
            Passionate about open source and developer experience, he has
            authored Pro Git and spoken globally on Git and software
            collaboration.
          </p>
          <div class="post-bio__links">
            <a href="#website">Website</a>
            <a href="#bluesky">Bluesky</a>
            <a href="#x">X</a>
          </div>
        </div>
      </div>
    </section>

    <PostsCarousel />
    <Subscribe />
    <Footer />
  </div>
</div>
