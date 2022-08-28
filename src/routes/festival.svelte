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
				<a href="https://forms.gle/D85ifeyFyKDfJYmk8">Volunteer to help out the festival here!</a>
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
			You can help too! <strong
				><a href="https://forms.gle/D85ifeyFyKDfJYmk8">Volunteer to help out the festival here</a
				></strong
			>
		</p>
	</div>
	<div class="box" id="values">
		<p class="title is-4">Meet the Department Leaders!</p>
		<div class="row-right">
			<div>
				<h5>Tom Yang (President)</h5>
				<p>
					Tom Yang, the project leader of the Chinese Festival, is also a competitive table tennis
					player. Recently, Tom Yang became the gold medalist in the Ontario Team Championship! In
					this Chinese Festival, he will be in charge of leading AIM and managing the festival
					departments to ensure the success of the Chinese Festival. He would host a meeting
					regularly for the department executives to ensure the functioning of the departments.
					Also, he created a welcoming letter for the festival, and helped CICSA translate, edit,
					and approve many important copywritings and documents.
				</p>
				<article class="message is-primary">
					<div class="message-body">
						I am very proud to be the leader of this project. I believe that all of us will
						collaborate at our best to host this festival. Everyone is important because the success
						of the festival will come with the contribution from each participant and volunteer. Not
						only will the Chinese Festival promote Chinese culture, but it also advocates certain
						measures to address the problem of climate change, namely, “zero-plastic life” and
						“low-carbon travel”. Additionally, we are grateful for the generous donations, as well
						as our sponsors who have supported us along the way. At last, I genuinely hope that our
						festival will run successfully, and I will give a huge thank you to every festival
						participant!!!
						<br /><br />
						—— Tom Yang
					</div>
				</article>
			</div>
			<img src="/tom-yang.png" alt="Tom Yang" />
		</div>
		<br />
		<div class="row-right">
			<div>
				<h5>Kevin Guo (Vice President)</h5>
				<p>
					Hey everyone! My name is Kevin, I’m a rising junior at the University of Toronto Schools,
					and I’m the Vice President of this Chinese Festival as well as the leader of the Sports
					Group. I’m currently a member of the U19 Canadian National Table Tennis team; last year, I
					represented Canada at the Pan American Junior Championships as part of the U15 team and I
					got the silver medal in the U15 Boys category at the Canadian National Table Tennis
					Championships.
				</p>
				<p>
					I enjoy learning and promoting Chinese culture, and I’m so happy to have the privilege of
					organizing this amazing event — the funds of which will all be donated to the Trillium
					Health Partners Foundation! I also want to bring more attention to some pressing issues
					that affect our current generation — these issues include the climate change crisis and
					the deterioration of mental health as a result of the pandemic — and to do this, I will be
					giving a speech at the Chinese Festival about climate change and I’ll be promoting sports
					clubs for youth to join as the pandemic begins to recede. Looking forward to seeing you
					all on September 17th!
				</p>
			</div>
			<img src="/kevin-guo.png" alt="Kevin Guo" />
		</div>
		<br />
		<div class="row-right">
			<div>
				<h5>Queena Qian (Vice President)</h5>
				<p>
					Hi, I am Queena Qian, a freshman in high school at Hillfield Strathallan College. I am the
					vice president of the Chinese Festival, and leader of the Art Department. From that, it is
					obvious that art is one of my favorite hobbies. I attended HSC@TheHelm, a monthly issue by
					the middle school in Hillfield Strathallan College as a comic illustrator. With my
					creativity, I was awarded with the 2022 D.C Willis Prize for Art. I also love nature
					and science, which is what I am truly passionate about. Other than that, I have been exploring the
					world of music along with my school band.
				</p>
			</div>
		</div>
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
