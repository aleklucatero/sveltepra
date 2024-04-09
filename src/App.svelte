<script>
    import { add } from "date-fns";

	let count = 0;
	function increment() {
		count = count + 1
	};

	/*---------Addint string to list----------*/

	let list = [`React`, `Vue`];
	function handleClick() {
		list = [...list, `Svelte`]
	};

	/*--------Adding number to list----------*/
   
	let items = [1, 2, 3, 4];
	$: amount = items.length;

	function addItems() {
		items = [...items, items.length + 1]
	}

	/*--------Adding a string----------*/
	let countries = [`USA`, `Mexico`];
	$: newCountry = countries[countries.length - 1];

	function addCountry() {
		countries = [...countries, `Italy`];
	}

</script>


<p class="first-button">Clicked {count} {count === 1  ? `time` : `times`}</p>
<button on:click={increment}>Click me</button>


<p class="second-button">{list}</p>
<button on:click={handleClick}>Update list</button>

<p class="items">The amount is {amount}</p>
<button on:click={addItems}>Add item</button>

<p>The new country is {newCountry}</p>
<button on:click={addCountry}>Add country</button>




<style>
	p.first-button {
		color: teal;
	}

	p.second-button {
		color: red;
	}

	.items {
		color: blue;
	}

</style>
