<script>
	import './styles.css';
	import Header from './Header.svelte';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<div class="end-text">
			<p>Copyright C @2023. All rights reserved. design by x</p>
		</div>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	.end-text {
		background-color: rgba(0, 0, 0, 0.26);
		text-align: center;
		padding: 0.1rem;
		opacity: 55%;
	}
	.end-text p {
		color: #000000;
		text-transform: capitalize;
		opacity: 100%;
	}
</style>
