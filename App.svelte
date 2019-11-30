<svelte:head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
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

  let state = {
    page: "start"
  }

  function showMenu(){
   
    state.page = "menu";
     console.log("showMenu called");
     //state = state;
  }

  function restart(){
    state.page = "start"
  }

</script>

<style>
  /* main {
                                    font-family: sans-serif;
                                    text-align: center;
                                  } */
  /* .container {
                              margin: 14px;
                            } */
</style>


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
<!-- 
<div class="container">
 <h1>SAGA (beta)</h1>
 <p>Interactive Fiction Engine</p>
 <em>by Andrew Wooldridge</em><br>
 <button class="button is-primary">Start</button>
 <button class="button is-link">Load</button>
</div> -->


<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a href="https://github.com/triptych/saga" class="navbar-item">SAGA</a>

    <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>

  </div>

  <div id="saga-main-navbar" class="navbar-menu">
    <div class="navbar-start">
      <a href="/"class="navbar-item">Home</a>
      <a href="#" class="navbar-item">Documentation</a>
      <a href="#" class="navbar-item">About</a>
    </div>
  </div>

</nav>

{#if state.page=="start"}
[start]
 <section class="section">
    <div class="container">
      <h1 class="title">
        SAGA Game Engine
      </h1>
      <p class="subtitle">
        Create Interactive Fiction in your browser!
      </p>
    </div>
    <div class="container">
      <a href="#" on:click|preventDefault="{showMenu}">
      Let's get started.
      <i class="fas fa-play"></i>
      
      </a>
    </div>
  </section>

{/if}

{#if state.page=="menu"}

<section class="section">
  <div class="container">
  [menu]
  <button on:click="{restart}">Back</button>

  </div>
</section>
{/if}