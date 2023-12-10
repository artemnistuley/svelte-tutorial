<script>
  let count = 0;
  const inc = () => count++;

  $: console.log(`1: the count is ${count}`);

  $: {
    console.log(`2: the count is ${count}`);
    console.log('this will also be logged.');
  };

  $: if (count >= 10) {
    count = 0;
  }
</script>

<button on:click={inc}>
  Clicked {count}
  {count === 1 ? 'time' : 'times'}
</button>
