<script>
	export let name;

	const tasks = ['wash car', 'mow lawn', 'cut hair'];
</script>

<main>
	<h1>Hello {name}</h1>
	<h2>To Do</h2>
	<ul>
		{#each tasks as task}
			<li>{task}</li>
		{/each}
	</ul>
</main>

<style>
	main {
		width: 100vw;
		height: 100vh;
		background-color: darkslateblue;
	}

	h1 {
		color: gold;
	}

	h2 {
		color: silver;
	}
</style>