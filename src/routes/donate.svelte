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
	<title>Donate</title>
	<meta name="description" content="As a non-for-profit organization, we can only continue to thrive with your help. Donations of any amount are appreciated. All donations we receive will be used to support the local community, and to allow us to host more cultural events in the future. Through donations, we are able to help more people, and achieve our mission of empowering the Chinese community in the Peel Region." />
</svelte:head>

<section class="hero is-primary">
	<div class="hero-body">
		<p class="title">Donate</p>
		<p class="subtitle">Help CISCA achieve its mission</p>
	</div>
</section>
<div class="content">
	<div class="box">
		<p>
			As a non-for-profit organization, we can only continue to thrive with your help. Donations of any amount are appreciated. All donations we receive will be used to support the local community, and to allow us to host more cultural events in the future. Currently, CICSA is focused on raising funds for Trillium Health Partners, a series of hospitals located in Mississauga. Through donations, we are able to help more people, and achieve our mission of empowering the Chinese community in the Peel Region.
		</p>

		<p>
			We accept donations through Interac E-Transfer to the email <a>info@mma99.com</a>
			<br />
			Thank you for supporting CISCA!
		</p>
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
