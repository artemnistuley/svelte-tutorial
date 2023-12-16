<script>
	import ComponentEventInner from "./ComponentEventInner.svelte";

	function handleMessage(event) {
		alert(event.detail.text);
	}
</script>

<ComponentEventInner on:btn-click={handleMessage} />
