<script>
  import Greeting from './Greeting.svelte';
  import LogIn from './LogIn.svelte';
  import FrameworkList from './FrameworkList.svelte';
  import EventDemo from './EventDemo.svelte';
  import BindingDemo from './BindingDemo.svelte';
  export let name;
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <h1>Hello {name}!</h1>
  <Greeting first_name="Alex" last_name="Gilliott" />
  <LogIn />
  <FrameworkList />
  <EventDemo />
  <BindingDemo />
</main>
