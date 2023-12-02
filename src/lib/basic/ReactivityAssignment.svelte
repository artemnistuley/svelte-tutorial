<script>
  let count = 0;

  const inc = () => count++;
</script>

<button on:click={inc}>
  Clicked {count}
  {count === 1 ? 'time' : 'times'}
</button>
