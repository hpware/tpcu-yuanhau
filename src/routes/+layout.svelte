<script lang="ts">
	import '../app.css';
	import githubimg from "/src/lib/images/github.svg";
	import Nav from './Nav.svelte';

	let { children } = $props();
</script>

<div class="app">
	<Nav/>

	<main>
		{@render children()}
	</main>
	<footer>
		<a href="https://github.com/hpware" target="_blank">
			<img src={githubimg} alt="github" width="32" height="32" />
		</a>
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

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
