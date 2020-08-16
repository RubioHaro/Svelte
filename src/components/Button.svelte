<script>
  export let count = 0;
  export let content;
</script>

<button on:click>{content}{count === 0 ? '' : count}</button>
