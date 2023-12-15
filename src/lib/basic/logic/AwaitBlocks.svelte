<script>
	async function fetchData() {
    const res = await fetch('https://swapi.dev/api/people/1');

    if (res.ok) {
      return await res.json();
    } else {
      // Sometimes the API will fail!
      throw new Error('Request failed');
    }
  }

  let promise = fetchData();
</script>

{#await promise}
  <p>waiting...</p>
{:then data} 
  {data.name}
{:catch error}
  <p style="color: red;">{error.message}</p>
{/await}
