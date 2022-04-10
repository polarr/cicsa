<script context="module" lang="ts">
	export const prerender = true;
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="CICSA is a registered Canadian not-for-profit charity organization. We offer social, artistic, cultural, educational, health and well-being support projects to assist new immigrants in integrating into Canada and achieving high quality of life within the community." />
</svelte:head>

<section>
	<section class="hero is-primary">
		<div class="hero-body">
			<div class="center-banner">
				<img
					src="/banner.jpeg"
					alt="logo"
				/>
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
							This summer, Canadian Innovative Community Services Alliance (CICSA), a charity
							organization, will host the Chinese Festival at Mississauga Celebration Square. While
							showcasing Chinese culture, the event will primarily promote ways of green living and
							concern adolescents' physical and mental development.
							<br /><br />
							In 2021, CICSA achieved its goal and donated to the Trillium Health Partners with support
							from the communities. In 2022, CICSA will continue to raise funds for Trillium Health Partners
							through various venues at the Chinese Festival. To closely follow the theme of this event,
							the Chinese Festival will have plenty of cultural events, sports activities, and entertainment
							- bicycle riding, buskers, children's playground, youth fitness, Chinese lantern riddles,
							and live performances. Let love sing aloud and comfort the soul with warmth.
							<br /><br />
							<a href="/festival">Learn more</a>
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
						As a non-for-profit organization, we can only continue to thrive with your help. Donations of any amount are appreciated. All donations we receive will be used to support the local community, and to allow us to host more cultural events in the future. Through donations, we are able to help more people, and achieve our mission of empowering the Chinese community in the Peel Region.
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
			margin: 0 .5rem;
		}
	}
</style>
