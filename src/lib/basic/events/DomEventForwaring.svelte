<script>
	import DomEventForwaringBtn from "./DomEventForwaringBtn.svelte";

	function handleClick() {
		alert('Clicked!')
	}
</script>

<DomEventForwaringBtn on:click={handleClick} />
