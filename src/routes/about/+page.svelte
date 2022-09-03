<main>
  <div class="master">
    <div class="logos">
      <img
        class="logo svelte-logo"
        src="/sveltekit-template/svg/svelte.svg"
        alt="Svelte logo"
      />
      <img
        class="logo vite-logo"
        src="/sveltekit-template/svg/vite.svg"
        alt="Vite logo"
      />
      <img
        class="logo ts-logo"
        src="/sveltekit-template/svg/typescript.svg"
        alt="Typescript logo"
      />
      <img
        class="logo prettier-logo"
        src="/sveltekit-template/svg/prettier.svg"
        alt="Prettier logo"
      />
    </div>
    <h1 class="head">About page</h1>
    <p class="body-txt">
      This is a template using Sveltekit, Prettier, Typescript, and Vite.
      <br />
      Also, this page is entirely HTML and CSS, with no JS involved.
    </p>
    <a href="/sveltekit-template">Back to home page</a>
  </div>
</main>

<style>
  .master {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 18px;
  }

  .head {
    margin: 0;
  }
  .body-txt {
    margin: 0;
    text-align: center;
    line-height: 1.5;
  }

  .logo {
    height: 128px;
  }

  .logos {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 24px;
  }

  .ts-logo:hover {
    filter: drop-shadow(0 0 2em #3178c6);
  }

  .vite-logo:hover {
    filter: drop-shadow(0 0 2em #666eff);
  }

  .svelte-logo:hover {
    filter: drop-shadow(0 0 2em #ff3e00);
  }

  .prettier-logo:hover {
    filter: drop-shadow(0 0 2em #bf85bf);
  }
</style>
