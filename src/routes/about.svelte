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
			description: "Respecting the dignity and self-worth of all individuals and recognizing their holistic needs. Enabling individuals to successfully direct their own lives independently and interdependently."
		}, 
		{
			value: "Collaboration",
			description: "Achieving success through working together with others on a mutual respect basis."
		}, 
		{
			value: "Volunteering",
			description: "Appreciating that the voluntary contributions of individuals contributes to the success of the organization and the community as a whole. Treating volunteers with utmost respect and support to facilitate volunteer work and growth."
		}, 
		{
			value: "Inclusivity",
			description: "Recognizing the diversity in the community and amongst our members, service users and volunteers. Providing culturally and linguistically appropriate service with a focus on the Chinese community."
		}, 
		{
			value: "Responsibility and Effectiveness",
			description: "Ensuring the organization will be managed and resources will be utilized in a responsible and effective manner." 
		}
	];
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About CICSA and its Vision, Mission, and Values" />
</svelte:head>

<section class="hero is-info">
	<div class="hero-body">
		<p class="title">About CICSA</p>
		<p class="subtitle">Our Mission, Values, and FAQ</p>
	</div>
</section>
<div class="content">
	<div class="box">
		<h1>About Us</h1>
		<div class="row-right">
			<p>
				CICSA, formerly known as the Mississauga Mandarin Association (MMA), stands for Canadian
				Innovative Community Services Alliance, and is a registered Canadian not-for-profit charity
				(BN: 863170320RR0001) organization. CICSA offers social, artistic, cultural, educational,
				health and well-being support projects to assist new immigrants in integrating into Canada and
				achieving high quality of life within the community.
			</p>
			<img src="/charity-heart.png" alt="Charity Heart" />
		</div>
	</div>
	<div class="box" id="mission">
		<h1>Vision & Mission</h1>
		<div class="row-right">
			<div>
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
			<img src="/hands-heart.jpg" alt="Hands Heart" />
		</div>
	</div>
	<div class="box" id="values">
		<h1>Values</h1>
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
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}

	img {
		height: 128px;
		padding: 1rem;
	}

	@media (max-width: 720px) {
		.row-right {
			flex-direction: column;
		}

		img {
			height: initial;
			width: 384px;
			padding: 1rem;
			margin: 0 auto;
		}
	}
</style>
