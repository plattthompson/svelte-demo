<script>
	import Monaco from './MonacoEditor.svelte';

	let monaco;
	window['monaco'] = monaco;
</script>

<section>
	<Monaco bind:this={monaco}/>
</section>

<style>
	section {
		grid-column: 6 / 21;
		grid-row: 3 / 25;
		display: flex;
		flex-flow: column nowrap;
		background-color: white;
	}
</style>