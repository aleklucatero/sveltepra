<script>
    import { each } from "svelte/internal";

    // import { lightFormat } from "date-fns";
    // import { filter } from "lodash-es";

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
	// function onSubmit() {
	// 	console.log(`Form submitted`);
	// }

	/*--------Data Binding, filterig list through search----------*/
	// let list = [`React`, `Vue`, `Svelte`];
	// let filteredList = [];
	// let searchQuery = ``;

	// function filterList() {
	// 	filteredList = list.filter(item => {
	// 		return item.toLowerCase().includes(searchQuery.toLowerCase());
	// 	});
	// }

	/*--------Components----------*/
	// import Artist from "./Artist.svelte"
	// import Album from "./Album.svelte"
	
	// let artist = [
	// 	{
	// 		name: `Fleetwood Mac`,
	// 		albums:  [
	// 			{
	// 				name: `Tango in the Night`,
	// 				year: 1987,
	// 				tracks: [
	// 					{ title: `Big Love`, length: `3:37` },
	// 					{ title: `Seven Wonders`, length: `3:38` },
	// 					{ title: `Everywhere`, length: `3:48` },
	// 					{ title: `Caroline`, length: `3:50` },
	// 					{ title: `Tango in the Night`, length: `3:56` },
	// 					{ title: `Mystified`, length: `3:08` },
	// 				]
	// 			}
	// 		]
	// 	}
	// ]

	/*--------Slots----------*/
	// import Button from "./Button.svelte"

	/*--------Animations----------*/
	// import { fade } from "svelte/transition";

	// let showFade = false
	
	// function toggleFade() {
	// 	showFade = !showFade
	// }

	/*--------Working with stores----------*/
	// import { message } from "./stores.js"

	// function updateStore() {
	// 	$message = `Bye`
	// }

	/*--------More Working with stores----------*/
	// import { localStorageStore } from "./stores.js"

	// let message = localStorageStore(`mesage`, `Hello`)

	// $message = `Bye`

	/*--------Social Media site----------*/
	let email = ``;
	let password = ``;

	function handleSubmit() {

	};



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
 
<!-- <form on:submit|preventDefault={onSubmit}>
	<input type="text">
	<button type="submit">Submit</button>
</form> -->

<!-- <input 
	on:input={filterList}
	bind:value={searchQuery}
	type="text"
/>

<ul>
	{#each filteredList as item}
		<li>{item}</li>
	{/each}
</ul> -->

<!-- {#each artist as artist}
	<Artist artistName={artist.name} />
		{#each artist.albums as album}
			<Album
				albumTitle={album.name}
				albumTracks={album.tracks}
			/>
		{/each}
{/each} -->

<!-- <Button>
	<span slot="icon">+</span>
	<span slot="text">Add</span>
</Button>

<Button>
	<span slot="icon">+</span>
	<span slot="text">Add</span>
</Button>

<Button>
	<span slot="icon">-</span>
	<span slot="text">Delete</span>
</Button> -->

<!-- <button on:click={toggleFade}>
	Wax poetic
</button>

{#if showFade}
	<blockquote transition:fade={{ delay: 250, duration: 300 }}>
		Memories fade, but friends are forever
	</blockquote>
{/if} -->

<!-- <p>{$message}</p>
<button on:click={updateStore}>Click</button> -->

<!-- {$message} -->

<style>
	.container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 100vh;
	}

	.left {
		width: 50%;
		padding: 0 2rem;
	}

	.right {
		width: 50%;
		padding: 0 2rem;
	}

	.logo {
		width: 80%;
		max-width: 300px;
		margin-bottom: 2rem;
	}

	form  {
		background-color: #f0f0f0;
		padding: 2rem;
		border-radius: 10px;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
	}
	
	input[type="email"],
	input[type="password"] {
		width: 100%;
		padding: 0.5rem;
		margin-bottom: 1rem;
		border: 1px solid #ccc;
		border-radius: 5px;
	}

	input[type="submit"] {
		width: 100%;
		padding: 0.75rem;
		background-color: #007bff;
		color: #fff;
		border: none;
		border-radius: 5px;
		cursor: pointer;
		transition: background-color 0.3s ease;
	}

	input[type="submit"]:hover {
		background-color: #0056b3;
	}


</style>

<div class="container">
    <div class="left">
        <img src="logo.png" alt="Social Media Logo" class="logo">
        <h1>Lorem Ipsum Dolor Sit Amet</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
    </div>
    <div class="right">
        <form on:submit|preventDefault={handleSubmit}>
            <h2>Login</h2>
            <input type="email" placeholder="Email" bind:value={email}>
            <input type="password" placeholder="Password" bind:value={password}>
            <input type="submit" value="Login">
        </form>
    </div>
</div>