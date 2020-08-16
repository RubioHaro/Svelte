<script>
  let text = `Iroh, Dragon del Oeste `;
  let count = 0;
  let styles = { darkMode: false };

  function toogle() {
    styles.darkMode = !styles.darkMode;
    window.document.body.classList.toggle("dark-mode");
  }

  function handleClick() {
    count++;
  }
</script>

<style>
  p {
    color: var(--theme-color);
  }
</style>

<div class="About">

  {#if !styles.darkMode}
    <p>{text}</p>
  {:else}
    <p>
      <span>El tio Iroh</span>
    </p>
  {/if}

  <button on:click={handleClick}>tés: {count == 0 ? '' : count}</button>
  <button on:click={toogle}>darkMode</button>
</div>
