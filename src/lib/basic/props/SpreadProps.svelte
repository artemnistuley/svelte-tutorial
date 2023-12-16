<script>
  import SpreadPropsNested from "./SpreadPropsNested.svelte";

  const pkg = {
    name: 'svelte',
    speed: 'blazing',
    version: 4,
    website: 'https://svelte.dev'
  };
</script>

<SpreadPropsNested {...pkg} testprop='testvalue' />
