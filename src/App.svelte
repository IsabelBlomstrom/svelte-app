<script>
	export let name;
	let count = 0;
	function handleClick() {
		count += 1;
	}
	</script>

<main>
	<h1>Hej {name}!</h1>
	<button on:click={handleClick}>
	Clicked {count}
	</button>
</main>

<style>

	main {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		padding: 1em;
		max-width: 240px;
		height: 100vh;
		margin: 0 auto;
		background-image: linear-gradient(to top, 
		#cd06b5, #ff0081, #ff5f4a, 
		#ffa40c, #ebde12);
	}

	h1 {
		color: black;
		text-transform: uppcercase;
		font-size: 4em;
		font-weight: 100;
	}

	button {
		border-radius: 2rem;
		padding: 1rem;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>