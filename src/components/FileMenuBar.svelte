<nav>
	<div>
		<button>File</button>
		<button>Edit</button>
		<button>Options</button>
		<button>Help</button>
	</div>
	<header>
		<h1>Svelte</h1>
	</header>
</nav>

<style>
	/*@import url('https://fonts.googleapis.com/css2?family=Jost&display=swap');*/

	nav {
		/*width: 100vw;*/
		/*height: 15vh;*/
		grid-column: 1 / 26;
		grid-row: 1 / 3;
		background-color: rosybrown;
		display: flex;
		flex-flow: row nowrap;
		/*justify-content: flex-start;
		align-items: center;*/
		justify-content: space-between;
		background-color: #060714;
		text-transform: uppercase;
		/*font-family: 'Jost', sans-serif;*/
	}

	div {
		width: 50vw;
	}

	button {
		/*width*/
		height: 100%;
		font-family: 'Jost', sans-serif;
		text-transform: uppercase;
	}

	header {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	h1 {
		margin: 0;
		padding: 0;
		/*font-family: 'Star Wars';*/
		font-family: 'Michroma', sans-serif;
		/*outlined*/
		color: #FFE81F;
	}
</style>