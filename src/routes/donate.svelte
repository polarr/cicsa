<script context="module">
	import { browser, dev } from '$app/env';
	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;
	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;
	export const prerender = true;

	const values = [
		{
			value: "People Focus",
			description: "Respecting the dignity and self-worth of all individuals and their holistic needs. Enabling individuals to successfully direct their own lives independently and interdependently."
		}, 
		{
			value: "Collaboration",
			description: "Achieving success through working together with others in the spirit of equal and mutual respect basis."
		}, 
		{
			value: "Volunteering",
			description: "Appreciating that the voluntary contribution of individuals contributes to the success of the organization and the community. Treating volunteers with utmost respect and support will be available to facilitate volunteer work and growth."
		}, 
		{
			value: "Inclusivity",
			description: "Recognizing the diversity in the community and amongst our members, service users and volunteers through the provision of culturally and linguistically appropriate service with the focus on the diversified Chinese community."
		}, 
		{
			value: "Responsibility and Effectiveness",
			description: "Ensuring the organization will be managed and resources will be utilized in a responsible and effective manner." 
		}
	];
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<section class="hero is-primary">
	<div class="hero-body">
		<p class="title">Donate</p>
		<p class="subtitle">Help CISCA achieve its mission</p>
	</div>
</section>
<div class="content">
	<div class="box">
		<h1>About Us</h1>
		<p>
			CICSA, formerly known as the Mississauga Mandarin Association (MMA), stands for Canadian
			Innovative Community Services Alliance, and is a registered Canadian not-for-profit charity
			(BN: 863170320RR0001) organization. CICSA offers social, artistic, cultural, educational,
			health and well-being support projects to assist new immigrants in integrating into Canada and
			achieving high quality of life within the community.
		</p>
	</div>
	<div class="box" id="mission">
		<h1>Our Vision & Mission</h1>
		<p>
			CICSA strives to be a productive agent to facilitate the establishing and sustaining of a
			vibrant and strong Chinese community in the Peel Region.
		</p>
		<p>
			Our mission is to empower Chinese people to settle and integrate in the Peel Region and to
			live a quality and enriched life in the community by providing a platform for civic engagement
			and participation and delivering a wide range of social, arts, cultural, education, health,
			and support programs.
		</p>
	</div>
	<div class="box" id="values">
		<h1>Our Values</h1>
		{#each values as value, i}
			<p class="title is-4">{value.value}</p>
			<ul><li>{value.description}</li></ul>
		{/each}
	</div>
	<div class="box" id="faq">
		<h1>FAQ</h1>
	</div>
</div>

<style>
	.content {
		width: 100%;
		padding: 0 1rem;
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
