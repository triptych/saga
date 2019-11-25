<script>
	let count = 0;

	function handleClick() {
	  count += 2;
	}
</script>

<style>
	/* button {
	  background: #ff3e00;
	  color: white;
	  border: none;
	  padding: 8px 12px;
	  border-radius: 2px;
	} */
</style>

<button on:click={handleClick} >
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>

{#if count > 1}
<a class="button is-primary is-small" id="newstim" title="New STIM">
				<span class="icon">
          <i class="fas fa-plus-square"></i>
        </span>
        <span> New STIM</span>
      </a>
{/if}