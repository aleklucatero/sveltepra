<script>
    import { each } from "svelte/internal";

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

	// let user = {
	// 	loggedIn: true
	// }

	// function toggle() {
	// 	user.loggedIn = !user.loggedIn;
	// };

	let todos = [
		{ id: 1, text: `Todo 1`, completed: true },
		{ id: 2, text: `Todo 2`, completed: false },
		{ id: 3, text: `Todo 3`, completed: false },
		{ id: 4, text: `Todo 4`, completed: false }
	]


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

<ul>
	{#each todos as todo}
		<li>
			<input checked={todo.comepleted} type="checkbox">
			<span>{todo.text}</span>
		</li>
	{/each}
</ul>