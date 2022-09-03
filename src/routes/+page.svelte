<script lang="ts">
  let count: number = 0;

  import { fly } from "svelte/transition";
</script>

<main>
  <div class="master">
    <img
      src="/sveltekit-template/svg/svelte.svg"
      alt="Svelte logo"
      class="logo"
    />
    <h1 class="head">Sveltekit Template</h1>
    <button on:click={() => count++}>
      <div>
        Count:
        {#key count}
          <span style="display: inline-block" in:fly={{ y: -20 }}>
            {count}</span
          >
        {/key}
      </div>
    </button>
    <button
      class="other-page-btn"
      on:click={() => (location.href = "/sveltekit-template/about")}
      >About page</button
    >
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

  .logo {
    height: 128px;
  }

  .logo:hover {
    filter: drop-shadow(0 0 2em #ff3e00);
  }
</style>
