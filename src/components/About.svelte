<script>
  let text = `Iroh, Dragon del Oeste `;
  let count = 0;

  function handleClick (){
    count++;
  }
</script>

<style>
  p {
    color: var(--theme-color);
  }
</style>

<div class="About">
  <p>{text}</p>
  <button on:click={handleClick}> tés: {count == 0 ? '' : count} </button>
</div>
