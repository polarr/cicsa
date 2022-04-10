<script context="module">
	import { browser, dev } from '$app/env';
	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;
	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;
	export const prerender = true;
</script>

<svelte:head>
	<title>Contact</title>
	<meta name="description" content="Contact information for CICSA" />
</svelte:head>

<section class="hero is-success">
	<div class="hero-body">
		<p class="title">
		Contact Us
		</p>
		<p class="subtitle">
		We'd love to hear from you!
		</p>
	</div>
</section>
<div class="content">
	<div class="box">
		<p class = "title is-4">Email</p>
		<p>Email us at <a href="mailto:cfestival@cicsa.ca">cfestival@cicsa.ca</a> if you have any questions or to share thoughts or concerns!</p>
	</div>
</div>

<style>
	.content {
		width: 100%;
		padding: 0 1rem;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
