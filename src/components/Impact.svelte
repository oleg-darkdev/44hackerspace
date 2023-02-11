<script>
	import { Card } from 'flowbite-svelte';
	import { CountUp } from 'countup.js';
	import { onMount } from 'svelte';

	onMount(() => {
		const boardgamesCountUp = new CountUp('boardgames', boardgamesCounter, {
				enableScrollSpy: true,
				duration: 8
			}),
			workshopsCountUp = new CountUp('workshops', workshopsCounter, {
				enableScrollSpy: true,
				duration: 12
			}),
			tournamentCountUp = new CountUp('tournament', tournamentsCounter, {
				enableScrollSpy: true,
				duration: 12
			}),
			toolsCountUp = new CountUp('tools', toolsCounter, { enableScrollSpy: true, duration: 12 });
	});

	const impactData = [
		{
			text: 'Gry planszowe są dostępne w bibliotece',
			id: 'boardgames',
			reverse: false,
			link: '/library',
			img: '/impact/boardgames.png'
		},
		{
			text: 'Narzędzi ręcznych i elektrycznych dostępnych dla klientów',
			id: 'tools',
			reverse: false,
			link: '/tools',
			img: '/impact/tools.png'
		},
		{
			text: 'Zorganizowaliśmy warsztatów',
			id: 'workshops',
			reverse: true,
			link: '#history',
			img: '/impact/workshops.png'
		},
		{
			text: 'Organizowane turnieje szachowych i warcabowych',
			id: 'tournament',
			reverse: true,
			link: 'https://yellow-elephant.vercel.app/',
			img: '/impact/tournament.png'
		}
	];

	export let tournamentsCounter, workshopsCounter, boardgamesCounter, toolsCounter;
</script>

<div style="justify-content: space-around;" class="mt-6 flex flex-wrap row w-full items-center">
	<h3 class="mb-2  text-4xl font-impact text-dark ">@44FabLab w liczbach</h3>
	{#each impactData as impact}
		<div class="w-full counter-card ">
			<!-- <Card  class="m-1" href={impact.link} img={impact.img} horizontal reverse={impact.reverse}>
                <h4 id={impact.id} class="mb-2 text-8xl font-bold tracking-tight text-viol dark:text-white"></h4>
                <p style="width: 300px;" class="mb-3 text-2xl font-normal text-violDark dark:text-gray-400 leading-tight">
                    {impact.text}
                </p>
            </Card> -->
			<a
				href={impact.link}
				class="flex max-w-sm flex-col-reverse md:flex-row-reverse md:max-w-xl bg-white dark:bg-gray-800 shadow-md text-gray-500 dark:text-gray-400 rounded-lg border border-gray-200 dark:border-gray-700 hover:bg-gray-100 dark:hover:bg-gray-700 m-1"
			>
				<img
					class="rounded-b-lg object-cover w-full h-48 md:h-auto md:w-48 md:rounded-none md:rounded-r-lg"
					src={impact.img}
					alt={impact.id}
				/>
				<div class="p-6">
					<h4
						id={impact.id}
						class="mb-2 text-8xl font-bold tracking-tight text-viol dark:text-white s-SoQEJKIKFvJc"
					/>
					<p
						style="width: 300px;"
						class="mb-3 text-2xl font-normal text-violDark dark:text-gray-400 leading-tight s-SoQEJKIKFvJc"
					>
						{impact.text}
					</p>
				</div>
			</a>
		</div>
	{/each}
</div>

<style>
	div .counter-card:nth-child(2n + 1) {
		display: flex;
		justify-content: end;
		padding-right: 10%;
	}
	div .counter-card:nth-child(2n) {
		display: flex;
		justify-content: start;
		padding-left: 10%;
	}
</style>
