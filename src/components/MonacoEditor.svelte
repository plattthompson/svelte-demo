<script context="module">
	let monaco_promise;
	let _monaco;

	monaco_promise = import('../monaco/monaco.js');
	monaco_promise.then(mod => {
		_monaco = mod.default;
	})
</script>

<script>
	import { onMount } from 'svelte';

	let monaco;
	let container;
	let editor;

	onMount(() => {
		if (_monaco) {
			monaco = _monaco;
			editor = monaco.editor.create(container);
		} else {
			monaco_promise.then(async mod => {
				console.log(container);
				monaco = mod.default;
				editor = monaco.editor.create(container, { value: 'check', language: 'python'});
			})
		}
		return () => {
			destroyed = true;
		}
	})
</script>

<div class="monaco-container" bind:this={container} style="height: 500px; text-align: left"></div>