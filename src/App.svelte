<script>
	let count = 0;
	function increment() {
		count = count + 1
	};

	/*------------------------*/

	let list = [`React`, `Vue`];
	function handleClick() {
		list = [...list, `Svelte`]
	}

</script>


<p class="first-button">Clicked {count} {count === 1  ? `time` : `times`}</p>
<button on:click={increment}>Click me</button>


<p class="second-button">{list}</p>
<button on:click={handleClick}>Update list</button>




<style>
	p.first-button {
		color: teal;
	}

	p.second-button {
		color: red;
	}


</style>
