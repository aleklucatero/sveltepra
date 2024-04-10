<script>
// import { errorToJSON } from "next/dist/server/render";
// import { each } from "svelte/internal";

    // import { add } from "date-fns";

	// let count = 0;
	// function increment() {
	// 	count = count + 1
	// };

	// /*---------Addint string to list----------*/

	// let list = [`React`, `Vue`];
	// function handleClick() {
	// 	list = [...list, `Svelte`]
	// };

	// /*--------Adding number to list----------*/
   
	// let items = [1, 2, 3, 4];
	// $: amount = items.length;

	// function addItems() {
	// 	items = [...items, items.length + 1]
	// }

	// /*--------Adding a string----------*/
	// let countries = [`USA`, `Mexico`];
	// $: newCountry = countries[countries.length - 1];

	// function addCountry() {
	// 	countries = [...countries, `Italy`];
	// }

	// /*--------Adding a string----------*/
	// let album = [
	// 	{track: `Track 1`, length: 180},
	// 	{track: `Track 2`, length: 240},
	// 	{track: `Track 3`, length: 280}
	// ]

	// $: albumLength = getAlbumLength(album)

	// function getAlbumLength(album) {
	// 	let lenghtSeconds = album.reduce((totalLength, currentValue) => {
	// 		return totalLength + currentValue.length
	// 	}, 0)

	// 	let [minutes, seconds] =
	// 	(lenghtSeconds / 60)
	// 	.toFixed(2)
	// 	.toString()
	// 	.split('.')

	// 	return { minutes, seconds };
	// };

	// function addTrack() {
	// 	album = [...album, {track: 'Track 4', length: 420}]

	// }

	/*--------Toggle Log in/ Log out button---------*/

	// let user = {
	// 	loggedIn: true
	// }

	// function toggle() {
	// 	user.loggedIn = !user.loggedIn;
	// };

	/*--------Iterating through list----------*/

	// let todos = [
	// 	{ id: 1, text: `Todo 1`, completed: true },
	// 	{ id: 2, text: `Todo 2`, completed: false },
	// 	{ id: 3, text: `Todo 3`, completed: false },
	// 	{ id: 4, text: `Todo 4`, completed: false }
	// ]

	/*--------Fetchin pokemon data----------*/
	// async function fetchPokemon(pokemonName) {
	// 	let url = `https://pokeapi.co/api/v2/pokemon/`;
	// 	let response = await fetch(`${url}${pokemonName}`);
	// 	let { name, sprites } = await response.json();

	// 	return {
	// 		name,
	// 		image: sprites['front_default']
	// 	}
	// }

	/*--------Using directives----------*/
	// let mouse = { x: 0, y: 0 };

	// function handleMouseMove(event) {
	// 	mouse.x = event.clientX
	// 	mouse.y = event.clientY
	// }

	/*--------Another example of using preventDefault----------*/
	function onSubmit() {
		console.log(`Form submitted`);
	}

</script>


<!-- <p class="first-button">Clicked {count} {count === 1  ? `time` : `times`}</p>
<button on:click={increment}>Click me</button>


<p class="second-button">{list}</p>
<button on:click={handleClick}>Update list</button>

<p class="items">The amount is {amount}</p>
<button on:click={addItems}>Add item</button>

<p>The new country is {newCountry}</p>
<button on:click={addCountry}>Add country</button>

<p>Album length is {albumLength.minutes} minutes and {albumLength.seconds} seconds.</p>
<button on:click={addTrack}>Add track</button> -->
 
<!-- {#if user.loggedIn}
	<button on:click={toggle}>Log Out</button>
{/if}

{#if !user.loggedIn}
	<button on:click={toggle}>Log In</button>
{/if} -->

<!-- <ul>
	{#each todos as { id, text, completed }, index(id)}
		<li>
			<input checked={completed} type="checkbox">
			<span>{text}</span>
		</li>
	{/each}
</ul> -->

<!-- {#await fetchPokemon('pikachu')}
	<p>Fetching data...</p>
{:then pokemon} 
	<h1>{pokemon.name}</h1>
	<img src={pokemon.image} alt={pokemon.name}>
{:catch error}
	<p>Something went wrong: {error.message}</p>
{/await} -->

<!-- <div on:mousemove={handleMouseMove}>
	The mouse position is {mouse.x} x {mouse.y}
</div>

<style>
	div {
		height: 100%;
	}
</style> -->
 
<form on:submit|preventDefault={onSubmit}>
	<input type="text">
	<button>Submit form</button>
</form>