<script lang="ts">
	import Navbar from '$lib/navbar/Navbar.svelte';
	import '../app.css';

</script>

<Navbar />

<main>
	<slot />
</main>

<footer class="footer">
	<div class="content has-text-centered">
		<p>
			Copyright © 2022-present CICSA
		</p>
	</div>
</footer>

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		width: 100%;
		margin:  3.25em auto;
		box-sizing: border-box;
		min-height: calc(100vh - 6.5rem);
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 40px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>
