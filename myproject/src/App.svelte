<script>
	let name="Lion";
	let FavColor="Blue";

	const Handle=()=>{
		FavColor="Yellow";
	}
	// const handleInput=(e)=>{
	// 	FavColor=e.target.value;
	// }
</script>

<main>
	<h1>Myself {name}!</h1>
	<p style="color: {FavColor}">{FavColor}</p>
	<button on:click={Handle}>Update Fav Color</button>
	<!-- For single way binding remove value -->
	<!-- <input type="text" on:input={handleInput} value={FavColor}> -->

	<input type="text" bind:value={FavColor}>

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		/* text-transform: uppercase; */
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>