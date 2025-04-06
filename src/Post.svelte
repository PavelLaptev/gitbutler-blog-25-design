<script lang="ts">
  import PostHero from "./lib/post/PostHero.svelte";
</script>

<PostHero />

<div class="content-wrap">
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
        <a
          class="post-share-btn blsk"
          href="#link"
          aria-label="Share on BlueSky"
        >
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
        <div class="post__table-of-contents-wrapper">
          <div class="post__table-of-contents">
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

        <p>
          If you interactive rebase, squash, fixup, and otherwise mangle your
          branch and someone wants to know the interdiff - the difference
          between the first version of your branch and a subsequent version, how
          do you find that difference? This is where git range-diff comes into
          play.
        </p>
        <p>
          There are a few different ways to run the command, but the simplest
          for this use case I think is the git range diff <base />
          <head-a>
            <head-b
              >. This calculates the range from both of the branch heads to the
              specified base, which gives you the two patch ranges you're trying
              to compare. Let's use a real-world, simple example.
            </head-b></head-a
          >
        </p>
      </section>
    </div>
  </div>
</div>
