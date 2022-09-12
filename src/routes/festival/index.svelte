<script context="module">
	import { browser, dev } from '$app/env';
	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;
	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;
	export const prerender = true;

	const supports = [
		'Title Sponsors (Finance, Food, Real Estate industry)',
		'Performance Sponsors (Groups or Individuals to perform in singing, dancing, etc.)',
		'Delicacies Sponsors (Ethnic food, family kitchen, drinks and more)',
		'Business Sponsors (Real Estates, Immigration, Insurance, Education, Outdoor sports)',
		'Culture Sponsors (Cultural heritage, geomancy, calligraphy)',
		'Farms and Gardens'
	];
</script>

<svelte:head>
	<title>Chinese Festival</title>
	<meta
		name="description"
		content="This summer, CICSA will host the Chinese Festival at Mississauga Celebration Square. The Chinese Festival will have plenty of cultural events, sports activities, and entertainment - bicycle riding, buskers, children's playground, youth fitness, Chinese lantern riddles, and live performances. While showcasing Chinese culture, the event will primarily promote ways of green living and concern adolescents' physical and mental development."
	/>
</svelte:head>

<section class="hero is-primary">
	<div class="hero-body">
		<p class="title">2022 Chinese Festival</p>
		<p class="subtitle">Cultural events, activities, and entertainment</p>
	</div>
</section>
<div class="content">
	<div class="box">
		<article class="message is-dark">
			<div class="message-body">
				Climate change is an issue that decides the features of this era, and we are now in this
				decisive moment.
				<br /><br />
				—— The United Nations
			</div>
		</article>
		<div class="row-right">
			<div>
				<p>
					Society changes rapidly. The notions of achieving sustainable living by low-carbon
					emissions, zero-plastic waste, and reduce-reuse-recycle system are pressing matters.
					Another imminent issue is the negative impact of COVID-19 on children and teenagers,
					including and its long-term psychological effects.
				</p>
				<p>
					This summer, Canadian Innovative Community Services Alliance (CICSA), a charity
					organization based in the Peel Region, will be hosting the Chinese Festival at Mississauga
					Celebration Square. While showcasing Chinese culture, the event will primarily promote
					ways of green living and address adolescents' physical and mental development. The Chinese
					Festival has garnered support from the Government of Canada, the Government of Ontario,
					and the Consulate General of China in Toronto. CICSA is grateful for their support, as
					well as encouragement and assistance from the City of Mississauga.
				</p>
			</div>
			<img src="/square-one.jpg" alt="Square One" />
		</div>
		<br />
		<p>
			<strong>
				Date: 9/17/2022
				<br />
				Location: Mississauga, Celebration Square One
				<br />
				<br />
				<a href="/festival/attractions">See all the events and attractions we have to offer!</a>
			</strong>
		</p>
	</div>
	<div class="box" id="values">
		<p class="title is-4">About the Festival</p>
		<div class="row-right">
			<div>
				<p>
					In 2021, CICSA achieved its goal and donated to the Trillium Health Partners with support
					from the communities. In 2022, CICSA will continue to raise funds for Trillium Health
					Partners through various venues at the Chinese Festival.
				</p>
				<p>
					No matter how the world changes, love is always the perpetual theme. The Chinese Festival
					will host charitable auctions at the event. The auctions will include but are not limited
					to crafts, art wares, and household items. We also anticipate artworks from different
					ethnic groups and products handmade by students.
				</p>
			</div>
			<img src="/trillium-health.png" alt="Trillium Health" />
		</div>
		<br />
		<p>
			The success of the 2022 Chinese Festival depends on the support from various communities. The
			CICSA Chinese Festival Committee hopes to receive support from
		</p>
		<ul>
			{#each supports as support, i}
				<li>{support}</li>
			{/each}
		</ul>
		<p>
			To closely follow the theme of this event, the Chinese Festival will have plenty of cultural
			events, sports activities, and entertainment - bicycle riding, buskers, children's playground,
			youth fitness, Chinese lantern riddles, and live performances. Let love sing aloud and comfort
			the soul with warmth.
		</p>
		<p>
			CICSA acknowledges the outstanding support from media in China and Canada. Hundreds of new
			outlets will make multiple perspective news reports on the Chinese Festival at the appointed
			date.
		</p>
		<p>
			<strong><a href="/festival/attractions">See all the events and attractions we have to offer!</a></strong>
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

	img {
		height: 256px;
		padding: 1rem;
		margin: 0 auto;
	}

	@media (max-width: 720px) {
		.row-right {
			flex-direction: column;
		}

		img {
			height: initial;
			width: 256px;
			padding: 1rem;
			margin: 0 auto;
		}
	}
</style>
