<script>
  let count = 0;
  $: doubled = count * 2;

  const inc = () => count++;
</script>

<button on:click={inc}>
  Clicked {count}
  {count === 1 ? 'time' : 'times'}
</button>

<p>{count} doubled is {doubled}</p>
