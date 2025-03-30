<section
  class="subscription"
  style="background-image: url('./subscribe-bg.svg')"
>
  <div class="subscription__text-wrap">
    <h2 class="subscription__title">Stay in the <i>Loop</i></h2>
    <p class="subscription__description">
      Subscribe to get fresh updates, insights, and exclusive content delivered
      straight to your inbox.<br />No spam, just great reads. 🚀
    </p>
  </div>

  <form
    class="subscription__form"
    action="https://app.gitbutler.com/api/v1/subscribe"
    method="POST"
  >
    <input
      type="email"
      name="email"
      placeholder="Your email address"
      required
      class="subscription__input"
    />
    <button type="submit" class="subscription__button">
      <div class="subscription__button-arrow">
        <svg viewBox="0 0 26 48" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M1.64526 1L24.0001 24L1.64526 47"
            fill="none"
            stroke="#000"
            stroke-width="2"
            vector-effect="non-scaling-stroke"
          />
        </svg>
      </div>
      <span>Subscribe</span>
    </button>
  </form>
</section>
