<script>
  import Button from "./Button.svelte";
  let state = {
    page: "two"
  };

  function show() {
    state.page = "one";
    console.log("one");
  }

  function hide() {
    state.page = "two";
    console.log("two");
  }
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }
</style>

<main>
	<h1>Hello CodeSandbox</h1>
	<h2>Start editing to see some magic happen!</h2>
	<Button />
<hr/>

{#if state.page =='two'}
  <button on:click={show}>show</button>
  {/if}
{#if state.page=='one'}  
  <button on:click={hide}>hide</button>
{/if}

</main>

