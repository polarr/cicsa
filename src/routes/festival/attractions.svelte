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
	<title>Chinese Festival</title>
	<meta
		name="description"
		content="This summer, CICSA will host the Chinese Festival at Mississauga Celebration Square. The Chinese Festival will have plenty of cultural events, sports activities, and entertainment - bicycle riding, buskers, children's playground, youth fitness, Chinese lantern riddles, and live performances. While showcasing Chinese culture, the event will primarily promote ways of green living and concern adolescents' physical and mental development."
	/>
</svelte:head>

<section class="hero is-primary">
	<div class="hero-body">
		<p class="title">2022 Chinese Festival</p>
		<p class="subtitle">Events and Attractions</p>
	</div>
</section>
<div class="content">
	<div class="box" id="about">
		<p class="title is-4">About</p>
		<div>
			<p>
				This year, the CICSA (Canadian Innovative Community Service Alliance) will be hosting a
				Chinese Festival on September 17, 2022, which will take place in Mississauga Celebration
				Square (300 City Centre Drive, Mississauga) from 11:00am-9:30pm. The primary themes of the
				festival will be climate change, youth mental health, and promotion of intangible Chinese
				culture. At the festival venue, there will be free milk tea, TCM treatment, a unique
				typography experience, and high-quality on-stage performances. The festival will raise funds
				for our partner: Trillium Health.
				<br /> <br />

				There will be 12 sections/types of booths in this charitable festival – stage, alcohol,
				business, food, mental health recovery and sport, pet adoption, hand-made craft, nursery
				garden/organic agriculture, education, children’s entertainment, mind yoga, poem, and
				intangible Chinese Cultural Heritage. The festival, which will have an expected turnout of
				over 10,000 individuals, has received donations and support from many different communities,
				sponsors, and individuals.
			</p>
		</div>
	</div>
	<div class="box">
		<aside class="menu">
			<p class="menu-label">Central Area</p>
			<ul class="menu-list">
				<li><a href="#central-area">Dekang Medical</a></li>
				<li><a href="#central-area">Art Auction</a></li>
				<li><a href="#central-area">Tradtional Typography Experience</a></li>
				<li><a href="#central-area">SIRUMEIRUO Chinese Traditional Costume</a></li>
				<li><a href="#central-area">Chinese Poetry</a></li>
			</ul>
			<p class="menu-label">Other Areas</p>
			<ul class="menu-list">
				<li><a href="#central-stage">Central Stage</a></li>
				<li><a href="#enterprise-exhibition">Enterprise Exhibition</a></li>
			</ul>
			<p class="menu-label">Youth Mental Health and Physical Recovery</p>
			<ul class="menu-list">
				<li><a href="#mental-health">Youth Mental Health and Physical Recovery</a></li>
			</ul>
		</aside>
	</div>
	<div class="box" id="central-area">
		<p class="title is-4">Central Area</p>
		<div>
			<p class="title is-5">Dekang Medical</p>
			<p>
				Dekang Medical has 4 traditional Chinese medical clinics in the Golden Horseshoe Area. Dr.
				Liang Gang, the founder of Dekang Medical, is working with three well-known acupuncture
				doctors at the Chinese Festival for free pulse checking of the festival’s attendees.
				Families are encouraged to accompany their elders to this amazing festival site to explore
				traditional Chinese methods of attaining longevity and preserving health.
			</p>
			<p class="title is-5">Art Auction</p>

			<p>
				The Chinese Festival committee has garnered support from members of the photography league,
				University of Rhode Island, OCAD, Sheridan College, Oakville Vision Art Academy, and
				individuals who have donated hundreds of pieces of artwork. All the artworks collected will
				go through an auction without a reserve price, and all revenue generated from the auction
				will be donated to Trillium Health Partners Foundation.
			</p>
			<p class="title is-5">Typography Experience</p>

			<p>
				Typography, one of the Four Great Inventions of China, has had a significant impact on the
				progress of civilization. In our Chinese festival a typography workshop called Wander on
				Paper will be inviting 100 visitors to experience typography for free. The experience will
				include learning about typography tools and how to selecting the appropriate content for
				printing. Participants will also learn about picking letters and applying ink to paper. This
				block will be a great opportunity for participants to experience the greatness of ancient
				China!
			</p>
			<p class="title is-5">Chinese Costume</p>
			<div class="row-right">
				<p>
					This traditional costume studio will provide Hanfu and other traditional dressing
					experiences. There will also be accessories displays, Hanfu performances, and Chinese
					Opera performances. The use of cameras is highly encouraged in order to capture the sheer
					beauty of this traditional Chinese culture. As participants marvel at the exquisite
					displays, they will feel as if they have physically travelled into Ancient China.
				</p>
				<img src="/chinese-costume.png" />
			</div>
			<p class="title is-5">Chinese Poetry</p>
			<p>
				At North square on the festival site, there will be Chinese poem performances brought by the
				Highland Voices Art Studio. Here, we will enjoy a peaceful moment, and listen to the voices
				from people who have lived centuries before us.
			</p>
		</div>
	</div>

	<div class="box" id="central-stage">
		<p class="title is-4">Central Stage</p>
		<div>
			<p>
				This event is also full of Chinese cultural performances and art showcases. Artists include
				but are not limited to GuQin Master: Long Wang, Action Artist & Celebrity stylist Yun: Feng
				Wan, well-known Chinese Opera segment- Yuji sword dancing by Echo Cultural art studio,
				YuanYin Guzheng studio for the Guzheng performance, Hanfu performance by Sirumeiruoxue Hanfu
				Studio, Sichuan Opera Bian Lian by Jessica & Andrew, U19 National table tennis exhibition
				match, Mississauga Chinese art ensemble dance performance, Yuzhengfang for the Guzheng
				performance, YangYang dance studio for the cultural dance performance, WeeKeeeeee B Band,
				YEZI MUSIC for the parent-child dance, cheongsam performance by Suzy Qipao studio, M-Dance
				Studio’s POP dance performance, Chinese poem reading, Performance by HSC student group,
				Shalala Yoga, etc. The hosts will introduce these performances in Mandarin, English, and
				French. Kevin Guo, the vice president of AIM and the Chinese Festival, will also be giving a
				speech at the festival to address climate change. All three levels of government in Canada
				will be on stage to support this charity event. BLACK IRIS STUDIO will be providing
				professional video/photo shooting full-time.
			</p>
			<p>
				Food is an important part of Chinese culture. There will be a variety of signature foods
				from all across China. Hungry Panda has invited Hero Milktea to sponsor 1200 cups of milk
				teas. At the same time, visitors can also have a taste of: Shanghai fried dim-sum, fried
				squid, Shanxi Rou Jia Mou, Sichuan cold dish, Northern-China BBQ, fried chicken, burgers,
				coffee, and Beavertails. This event has ACCO permission from the provincial government and
				the permission of legal alcohol. In front of the stage, there will be an alcohol area hosted
				by Jane He, with all profits donated to the Trillium Health Partners. While watching the
				performances and enjoying the food and drinks, you are also helping charities thrive.
			</p>
		</div>
	</div>

	<div class="box" id="enterprise-exhibition">
		<p class="title is-4">Enterprise Exhibition</p>
		<div>
			<p>
				This event is also full of Chinese cultural performances and art showcases. Artists include
				but are not limited to GuQin Master: Long Wang, Action Artist & Celebrity stylist Yun: Feng
				Wan, well-known Chinese Opera segment- Yuji sword dancing by Echo Cultural art studio,
				YuanYin Guzheng studio for the Guzheng performance, Hanfu performance by Sirumeiruoxue Hanfu
				Studio, Sichuan Opera Bian Lian by Jessica & Andrew, U19 National table tennis exhibition
				match, Mississauga Chinese art ensemble dance performance, Yuzhengfang for the Guzheng
				performance, YangYang dance studio for the cultural dance performance, WeeKeeeeee B Band,
				YEZI MUSIC for the parent-child dance, cheongsam performance by Suzy Qipao studio, M-Dance
				Studio’s POP dance performance, Chinese poem reading, Performance by HSC student group,
				Shalala Yoga, etc. The hosts will introduce these performances in Mandarin, English, and
				French. Kevin Guo, the vice president of AIM and the Chinese Festival, will also be giving a
				speech at the festival to address climate change. All three levels of government in Canada
				will be on stage to support this charity event. BLACK IRIS STUDIO will be providing
				professional video/photo shooting full-time.
			</p>
			<p>
				Food is an important part of Chinese culture. There will be a variety of signature foods
				from all across China. Hungry Panda has invited Hero Milktea to sponsor 1200 cups of milk
				teas. At the same time, visitors can also have a taste of: Shanghai fried dim-sum, fried
				squid, Shanxi Rou Jia Mou, Sichuan cold dish, Northern-China BBQ, fried chicken, burgers,
				coffee, and Beavertails. This event has ACCO permission from the provincial government and
				the permission of legal alcohol. In front of the stage, there will be an alcohol area hosted
				by Jane He, with all profits donated to the Trillium Health Partners. While watching the
				performances and enjoying the food and drinks, you are also helping charities thrive.
			</p>
		</div>
	</div>
	<div class="box" id="mental-health">
		<p class="title is-4">Youth Mental Health and Physical Recovery</p>
		<div>
			<p>
				Many related booths spread out throughout the event site are set up for the second theme of
				the Chinese Festival, which is youth mental health. These booths include the Arctic
				snowboard club, Canada CELPIP Education Center, Spirit of Pentecost, Three 10 Table Tennis
				Club, So Golf Academy, 4UBadminton Center, Love Swimming Private School, Mississauga Hockey
				League, AM PET, Save Fur Pets, Paws Love Pet Food, UTM CSSA, Mounsea Studio, Icon Studio
				Icon, Ethan&Judy Studio, UFORSE EDUCATION GROUP, and chameleonslimes.com. There will also be
				plenty of fun activities in the children’s area, such as water fountains, trampolines,
				popcorn, face painting, chalk floor painting, and handicraft. Since parents also need to
				rest during the festival, the organizers of the festival have planned a mind garden on the
				west side of North Square for a special spiritual experience led by Sharala Yoga Meditation
				Display and Teaching.
			</p>
			<p>
				In terms of fresh produce, the Capony Garden, which carefully cultivates various precious
				peony varieties so that the peony will still grow in the winter, will have a booth at the
				festival; moreover, Skyland Farm and Veggy-Symphony Mushroom Farm will be providing everyone
				with agricultural products favored by many Chinese. The 2022 Chinese Festival charity event
				is a grand celebration of traditional Chinese culture. Through this event, we aspire to
				propagate our traditional culture, provide assistance and support to the future generation,
				and advocate a greener life and eco-friendly practices.
			</p>
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
