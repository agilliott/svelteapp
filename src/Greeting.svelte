<script>
  export let first_name;
  export let last_name;

  $: name = first_name + ' ' + last_name;
</script>

<style>
  h2 {
    color: grey;
    font-weight: 200;
  }
</style>

<h2>Love from {name}</h2>
