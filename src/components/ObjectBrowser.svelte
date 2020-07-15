<script>
	import Fa from 'svelte-fa';
	import { faPlus, faPen, faEye } from '@fortawesome/free-solid-svg-icons';
	import ObjectTab from './ObjectTab.svelte';

	const galaxy = [];

	const planets = [
		{name: 'Naboo', id: 1},
		{name: 'Kashyyyk', id: 2}
	]

	const spacecraft = [
		{name: 'Millennium Falcon', id: 12},
		{name: 'X-Wing', id: 100},
		{name: 'TIE Fighter', id: 66}
	]
</script>

<section>
	<div class="object-browser-header-container">
		<h2>Object Browser</h2>
		<div class="object-browser-icons">
			<Fa icon={faPlus} class="object-browser-icon"/>
			<Fa icon={faPen} class="object-browser-icon"/>
			<Fa icon={faEye} class="object-browser-icon"/>
		</div>
	</div>
	<div class="object-tabs">
		<ObjectTab name="A Galaxy Far, Far Away" tab={galaxy}/>
		<ObjectTab name="Planet Stations" tab={planets}/>
		<ObjectTab name="Spacecraft" tab={spacecraft}/>
	</div>
</section>


<style>
	section {
		grid-column: 1 / 6;
		grid-row: 3 / 25;
		display: flex;
		flex-flow: column nowrap;
		justify-content: space-between;
		background-color: gray;
		font-family: 'Jost', sans-serif;
	}

	.object-browser-header-container {
		display: flex;
		flex-flow: row nowrap;
	}

	h2 {
		color: #36DAF9;
		/*color: #13F3FE;*/
		/*color: #10F1FF;*/
		color: #16F8FE;
	}

	.object-browser-icons {
		display: flex;
		flex-flow: row nowrap;
		justify-content: center;
		align-items: center;
		color: white;
	}

	/*.object-browser-icon:hover {
		cursor: pointer;
	}*/

	h3 {
		margin: 0;
		padding: 0;
	}

	.object-tab {
		display: flex;
		flex-flow: row nowrap;
	}
</style>