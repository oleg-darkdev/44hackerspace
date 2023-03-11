<script>
	import WhatWeDoCard from './bio/WhatWeDoCard.svelte';
	import PaperYellow from '../layout/PaperYellowSetcionWrapper.svelte';
	import BioCard from '../components/bio/BioCard.svelte';
	import Impact from '../components/Impact.svelte';

	const WhatWeDoInfo = [
		{
			heading: 'Warsztat z narzędziami ręcznymi i elektrycznymi',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: false,
			img: '/about/boardgames.png',
			link: '/library'
		},
		{
			heading: 'Druk 3d',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: false,
			img: '/about/3d.png',
			link: '/workshop#printer'
		},
		{
			heading: 'Wycinanie i grawerowanie laserowe',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: true,
			img: '/about/laser.png',
			link: '/workshop#laser'
		},
		{
			heading: 'Stacja naprawy rowerów',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: true,
			img: '/about/boardgames.png',
			link: '/library'
		},
		{
			heading: 'Wypożyczalnia gier planszowych',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: false,
			img: '/about/boardgames.png',
			link: '/library'
		},
		{
			heading: 'Turnieje szachowe',
			description:
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			reverse: true,
			img: '/about/chess.png',
			link: 'https://yellow-elephant.vercel.app/'
		}
	];

	const DescriptionText = [
		{
			heading: 'Z Białorusi z miłością',
			description:
				'Przestrzeń, stworzona przez uchodźcę politycznego z Białorusi, z myślą do wspólnej twórczości i technicznej edukacji.'
		},
		{
			heading: 'Edukacyjne gry planszowe',
			description:
				'Popularyzacja edukacyjnych gier planszowych, projektowanie i wykonywanie własnych gier planszowych.'
		},
		{
			heading: 'Dostępność dla wszystkich',
			description:
				'Bardzo zależy na tym, aby przestrzeń była przyjazna i otwarta dla jak najszerszej grupy odbiorców. Także dla uchodźców z krajów byłego Związku Radzieckiego.'
		},
		{
			heading: 'Otwarte warsztaty',
			description:
				'Tematyka tradycyjnie pokrywa się z szeroko pojętym IT, programowaniem, Open Source, elektroniką oraz CNC, 3D.'
		}
	];

	export let tournamentsCounter, workshopsCounter, boardgamesCounter, toolsCounter;
</script>

<div
	class="w-12/12  md:-mt-52 lg:-mt-52 xl:-mt-52 -mt-16 -mb-52 flex flex-row justify-center flex-wrap "
>
	<PaperYellow>
		<a name="mission" />
		{#each DescriptionText as text}
			<BioCard {text} />
		{/each}

		<a name="stats" />
		<Impact {tournamentsCounter} {workshopsCounter} {boardgamesCounter} {toolsCounter} />
	</PaperYellow>
</div>

<div
	class="w-12/12 mt-52 flex flex-col pb-12 pt-12 items-center flex-wrap"
	style="background-color: #f3e600;"
>
	<a name="service" />

	<h2 class="lg:text-7xl text-5xl text-center mb-2 text-dark font-impact">Dostępne dla gości</h2>
	<div class="flex flex-wrap w-full flex-row justify-center">
		{#each WhatWeDoInfo as weDo}
			<WhatWeDoCard
				heading={weDo.heading}
				description={weDo.description}
				img={weDo.img}
				reverse={weDo.reverse}
				href={weDo.link}
			/>
		{/each}
	</div>
</div>
