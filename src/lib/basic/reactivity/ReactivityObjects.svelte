<script>
	let numbers = [1, 2, 3, 4];
  let users = {
    user1: { name: 'Joe' },
  };

	function addNumber() {
    numbers = [...numbers, numbers.length + 1];
	}

  function addUser() {
    users.user2 = { name: 'Doe' };
  }

	$: sum = numbers.reduce((total, currentNumber) => total + currentNumber, 0);
  $: usersStr = JSON.stringify(users);
</script>

<p>{numbers.join(' + ')} = {sum}</p>

<button on:click={addNumber}>
	Add a number
</button>

<p>{usersStr}</p>

<button on:click={addUser}>
	Add user
</button>
