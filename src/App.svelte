<script>
	import FileMenuBar from './components/FileMenuBar.svelte';
	import ObjectBrowser from './components/ObjectBrowser.svelte';
	import ScriptEditor from './components/ScriptEditor.svelte';
	import ScriptElementsMenu from './components/ScriptElementsMenu.svelte';
</script>

<main>
	<FileMenuBar/>
	<ObjectBrowser/>
	<ScriptEditor/>
	<ScriptElementsMenu/>
</main>

<svelte:head>
	<link rel="stylesheet" type="text/css" href="https://fonts.googleapis.com/css2?family=Jost&display=swap">
	<link href="https://fonts.googleapis.com/css2?family=Michroma&display=swap" rel="stylesheet">
</svelte:head>

<style>
	main {
		width: 100vw;
		height: 100vh;
		display: grid;
		grid-template-columns: repeat(24, 1fr);
		grid-template-rows: repeat(24, 1fr);
		/*background-color: darkslateblue;*/
	}
</style>