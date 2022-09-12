<script context="module" lang="ts">
	export const prerender = true;
</script>

<svelte:head>
	<title>Home</title>
	<meta
		name="description"
		content="CICSA is a registered Canadian not-for-profit charity organization. We offer social, artistic, cultural, educational, health and well-being support projects to assist new immigrants in integrating into Canada and achieving high quality of life within the community."
	/>
</svelte:head>

<section>
	<section class="hero is-primary">
		<div class="hero-body">
			<div class="center-banner">
				<img src="/banner.jpeg" alt="logo" />
			</div>
		</div>
	</section>

	<div class="tile is-ancestor is-12 is-flex-wrap-wrap">
		<div class="tile is-vertical is-8">
			<div class="tile is-parent">
				<article class="tile is-child notification is-primary">
					<p class="title">2022 Chinese Festival</p>
					<p class="subtitle">Cultural events, activities, and entertainment</p>
					<div class="row-right">
						<div class="content">
							This year, the CICSA (Canadian Innovative Community Service Alliance) will be hosting
							a Chinese Festival on September 17, 2022, which will take place in Mississauga
							Celebration Square (300 City Centre Drive, Mississauga) from 11:00am-9:30pm. The
							primary themes of the festival will be climate change, youth mental health, and
							promotion of intangible Chinese culture. At the festival venue, there will be free
							milk tea, TCM treatment, a unique typography experience, and high-quality on-stage
							performances. The festival will raise funds for our partner: Trillium Health. 
							<br /> <br />
							There will be 12 sections/types of booths in this charitable festival - stage, alcohol,
							business, food, mental health recovery and sport, pet adoption, hand-made craft,
							nursery garden/organic agriculture, education, children's entertainment, mind yoga,
							poem, and intangible Chinese Cultural Heritage. The festival, which will have an
							expected turnout of over 10,000 individuals, has received donations and support from
							many different communities, sponsors, and individuals.
							<br /><br />
							<a href="/festival">Learn more</a>
							<br />
							<strong><a href="/festival/attractions">See all the events and attractions we have to offer!</a></strong>

						</div>
						<img src="/square-one.jpg" alt="Square One" />
					</div>
				</article>
			</div>
			<div class="tile is-parent">
				<article class="tile is-child notification is-success">
					<div class="content">
						<p class="title">Local News</p>
					</div>
				</article>
			</div>
		</div>
		<div class="tile is-vertical">
			<div class="tile is-parent">
				<article class="tile is-child notification is-info">
					<p class="title">About CICSA</p>
					<div class="content">
						CICSA is a registered Canadian not-for-profit charity organization. We offer social,
						artistic, cultural, educational, health and well-being support projects to assist new
						immigrants in integrating into Canada and achieving high quality of life within the
						community.
						<br /><br />
						<a href="/about">Learn more</a>
					</div>
				</article>
			</div>
			<div class="tile is-parent">
				<article class="tile is-child notification is-warning">
					<p class="title">Donate</p>
					<p class="subtitle">Help CICSA achieve its mission</p>
					<div class="content">
						As a non-for-profit organization, we can only continue to thrive with your help.
						Donations of any amount are appreciated. All donations we receive will be used to
						support the local community, and to allow us to host more cultural events in the future.
						Through donations, we are able to help more people, and achieve our mission of
						empowering the Chinese community in the Peel Region.
						<br /><br />
						<a href="/donate">Donate</a>
					</div>
				</article>
			</div>
			<div class="tile is-parent">
				<article class="tile is-child notification is-danger">
					<p class="title">Contact Us</p>
					<p class="subtitle">We'd love to hear from you!</p>
					<div class="content">
						Don't hesitate to email us at <a href="mailto:cfestival@cicsa.ca">cfestival@cicsa.ca</a>
						if any questions arise or to share your thoughts/concerns.
					</div>
				</article>
			</div>
		</div>
	</div>
</section>

<style lang="scss">
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0;
		color: #fff;
	}

	h1 {
		width: 100%;
	}

	.hero {
		background-color: #fff;
		margin-bottom: 3.25rem;
	}

	.hero-body {
		img {
			width: clamp(0px, 30%, 480px);
			display: block;
			padding: initial;
		}
	}

	.center-banner {
		width: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	img {
		width: 256px;
		padding: 0 1rem 1rem 1rem;
	}

	@media (max-width: 1080px) {
		.row-right {
			flex-direction: column;
		}

		img {
			height: initial;
			width: 512px;
			padding: 1rem;
			margin: 0 auto;
		}
	}

	@media (max-width: 768px) {
		.tile.is-ancestor {
			margin: 0 0.5rem;
		}
	}
</style>
