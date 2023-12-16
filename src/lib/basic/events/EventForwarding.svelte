<script>
  import EventForwardingOuter from "./EventForwardingOuter.svelte";

  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<EventForwardingOuter on:btn-click={handleMessage} />
