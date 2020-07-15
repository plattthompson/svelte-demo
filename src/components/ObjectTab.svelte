<script>
	import Fa from 'svelte-fa';
	import { faChevronDown } from '@fortawesome/free-solid-svg-icons';

	export let name;
	export let tab;
</script>

<div class="object-tab">
	<h3>{name}</h3>
	<Fa icon={faChevronDown}/>
</div>
{#if tab.length > 0}
	<ul>
		{#each tab as subtab (subtab.id)}
			<li>{subtab.name}</li>
		{/each}
	</ul>
{/if}