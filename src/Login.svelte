<script>
  let user = { loggedIn: false };

  function toggle() {
    user.loggedIn = !user.loggedIn;
  }
</script>

<style>
  button {
    background: transparent;
    border: 1px solid #ff3e00;
    color: #ff3e00;
  }
</style>

<p>
  You are logged
  {#if !user.loggedIn}out{:else}in{/if}
</p>
<button on:click={toggle}>
  {#if user.loggedIn}Log Out{/if}
  {#if !user.loggedIn}Log In{/if}
</button>
