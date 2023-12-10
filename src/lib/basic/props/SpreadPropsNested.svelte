<script>
  export let name;
  export let version;
  export let speed;
  export let website;

  console.log($$props);
</script>

<p>
  {name} <br />
  {version} <br />
  {speed} <br />
  {website}
</p>
