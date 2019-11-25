<svelte:head>
	<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.5/css/bulma.min.css" />
	<script defer src="https://use.fontawesome.com/releases/v5.3.1/js/all.js"></script>
</svelte:head>

<script>
  import Button from "./Button.svelte";
  // let state = {
  //   page: "two"
  // };

  // function show() {
  //   state.page = "one";
  //   console.log("one");
  // }

  // function hide() {
  //   state.page = "two";
  //   console.log("two");
  // }

</script>

<style>
  /* main {
          font-family: sans-serif;
          text-align: center;
        } */
  .container {
    margin: 14px;
  }
</style>

<main>
	<!-- <h1>Hello CodeSandbox</h1>
	<h2>Start editing to see some magic happen!</h2>
	<Button />
<hr/>

{#if state.page =='two'}
  <button on:click={show}>show</button>
  {/if}
{#if state.page=='one'}  
  <button on:click={hide}>hide</button>
{/if} -->

<!-- <Button type="is-primary">I'm a Button!</Button> -->
<!-- 
<div class="buttons">
  <button class="button is-primary">Primary</button>
  <button class="button is-link">Link</button>
</div>

<div class="buttons">
  <button class="button is-info">Info</button>
  <button class="button is-success">Success</button>
  <button class="button is-warning">Warning</button>
  <button class="button is-danger">Danger</button>
</div> -->

<!-- 

      <Button/> -->

<div class="container">
 <h1>SAGA (beta)</h1>
 <p>Interactive Fiction Engine</p>
 <em>by Andrew Wooldridge</em><br>
 <button class="button is-primary">Start</button>
 <button class="button is-link">Load</button>
</div>
</main>

