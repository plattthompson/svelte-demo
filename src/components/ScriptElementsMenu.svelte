<script>
	const exampleElements = ['one fish', 'two fish', 'red fish', 'blue fish']
</script>

<section>
	<div>
		<h2>Script Elements</h2>
	</div>
	<ul>
		{#each exampleElements as element}
			<li>{element}</li>
		{/each}
	</ul>
</section>

<style>
	section {
		grid-column: 21 / 25;
		grid-row: 3 / 25;
		background-color: cornflowerblue;
	}
</style>