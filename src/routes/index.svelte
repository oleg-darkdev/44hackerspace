<script>
	import Carousel from '../components/Carousel.svelte';
	import WorkshopCard from '../components/WorkshopCard.svelte';
	import Contact from '../components/Contact.svelte';
	import Bio from '../components/Bio.svelte'; 
	import YellowSetcionWrapper from '../layout/YellowSetcionWrapper.svelte';
	import BoardgamesList from '../components/BoardgamesList.svelte';
	import socialCordinatorLinks from '../data/socialCordinatorLinks';
	// import socialHackerspaceLinks from '../data/socialHackerspaceLinks';

	const workshopsList = [
		{
			title: 'Turnieje szachowe',
			description: [
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			],
			img: '/workshops/workshop_chess.png',
			partners: [
				{
					logo: '/partners/partner_44_cubes.svg',
					link: '',
					title: ''
				},
				{
					logo: '/partners/partner_darkdev.svg',
					link: '',
					title: ''
				},
			],
			harmonogram: [
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
			]
		},
		{
			title: 'Naprawa rowerów w hackerspace',
			description: [
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			],
			img: '/workshops/workshop_bicycle.png',
			partners: [
				{
					logo: '',
					link: '',
					title: ''
				}
			],
			harmonogram: [
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
			]
		},
		{
			title: 'Zagrajmy razem w gry planszowe',
			description: [
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			],
			img: '/workshops/workshop_boardgames.png',
			partners: [
				{
					logo: '',
					link: '',
					title: ''
				}
			],
			harmonogram: [
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
			]
		},
		{
			title: 'Naprawa domowych urządzeń elektrycznych',
			description: [
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			],
			img: '/workshops/workshop_electric.png',
			partners: [
				{
					logo: '',
					link: '',
					title: ''
				}
			],
			harmonogram: [
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
			]
		},
		{
			title: 'Ręcznie wyrabiane gier planszowych',
			description: [
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
				'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
			],
			img: '/workshops/workshop_boardgames_diy.png',
			partners: [
				{
					logo: '',
					link: '',
					title: ''
				}
			],
			harmonogram: [
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
				{
					date: '22.02.2022',
					linkFb: '',
					linkTg: '',
					img: '',
					title: 'Neil Sims'
				},
			]
		},
	];
</script>



<Carousel />

<section class="bio-section"> 
	<Bio />
</section>

<!-- <section class="boardgames-section mb-24 mt-24" > 
	<a name="boardgames"></a> 
	<BoardgamesList />
</section> -->

<section class="flex  bg-white pt-12 justify-center flex-col items-center pb-14">
	<a name="workshops"></a>
	<h2 class="lg:text-7xl text-5xl text-center text-dark font-black">Lista warsztatów</h2>
		{#each workshopsList as workshop}
			<WorkshopCard {workshop}/>
		{/each}
</section>

<!-- <section class="tools-section mb-24 mt-24">
<a name="tools"></a>

</section> -->


<!-- <section class="workshops-section mb-24 mt-24">
<a name="tools"></a>


</section> -->




<!-- <section class="faq-section mb-24 mt-24">
<a name="faq"></a>

</section> -->


<section class="bg-dark p-12 h-auto lg:w-12/12 px-8 sm:w-12/12  flex flex-col justify-center content-center ">
<a name="contact"></a>
	<h2
		class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-white md:text-5xl lg:text-6xl text-center"
	>
		Skontaktuj się z nami
	</h2>
	<div
		style="max-width: 100%;"
		class="mb-4 max-w-sm bg-current flex flex-col items-center shadow-md rounded-lg border border-current  text-gray-500 p-6"
	>
		<div class="m-4 lg:w-6/12 md:w-8/12 w-12/12 flex flex-wrap justify-center flex-row bg-dark p-6 rounded-3xl">
			<h5 class="mb-2 text-2xl font-bold tracking-tight  text-white text-center">
				44hackerspace@gmail.com
			</h5>
			<h5 class="mb-2 text-2xl font-bold tracking-tight  text-white text-center">
				Mazowiecka 26, 81-862 Sopot, Poland
			</h5>
			<!-- добавить блок координатора проекта из itingo -->
			<div  class="border border-white  flex max-w-sm flex-col m-2  dark:bg-gray-800 shadow-md text-gray-500 dark:text-gray-400 rounded-lg  dark:border-gray-700">
    <img loading="lazy" class="rounded-t-lg" src="/coordinator.png" alt=""> 

				<div class="p-1 rounded bg-lightYellow">
    <h5 class="mb-1 text-2xl font-bold text-center tracking-tight text-white">
      Koordynator projektu
    </h5> 
    <p class="mb-3 text-4xl font-black text-center text-white">
      Oleg Medvedev
    </p>
	<div class="flex flex-wrap justify-center flex-row ">
		<a href="{socialCordinatorLinks.facebook}">
			<img src="social/facebook.svg" class="w-15 h-15 rounded" alt="facebook">

		</a>
		<a href="{socialCordinatorLinks.github}">
			<img src="social/github.svg" class="w-15 h-15 rounded" alt="github">

		</a>
		<a href="{socialCordinatorLinks.linkedin}">
			<img src="social/linkedin.svg" class="w-15 h-15 rounded" alt="linkedin">

		</a>
		<a href="{socialCordinatorLinks.github}">
			<img src="social/patronite.svg" class="w-15 h-15 rounded" alt="patronite">

		</a>
		<a href="">
		<img src="social/telegram.svg" class="w-15 h-15 rounded" alt="telegram">

		</a>
	</div>

    <!-- <div style="" class="border-viol wrap-social-container mb-4 flex-col items-center justify-center">
    <div class="social-coordinator-container">
        <a target="_blank" href="https://www.facebook.com/hulio.mondre"><i class="icon-facebook fb-mode "></i></a>
        <a  target="_blank" href="https://www.linkedin.com/in/oleg-darkdev"><i class="icon-linkedin ln-mode "></i></a> 
        <a target="_blank" href="https://github.com/oleg-darkdev"><i class="icon-github gh-mode "></i></a>

    </div>
	
    <h2 class="w-full text-center text-3xl text-viol font-black m-0"><i class="icon-hand-up text-viol"></i> w mediach <i class="icon-hand-up text-viol"></i></h2>
</div> -->


  </div>
</div>


			
		</div>

		
		<Contact />



			<iframe
				class="m-2 bg-white shadow-md rounded-lg border border-gray-200 text-gray-500 p-2"
				width="100%"
				height="600px"
				frameborder="0"
				scrolling="no"
				marginheight="0"
				marginwidth="0"
				src="https://www.openstreetmap.org/export/embed.html?bbox=18.547909855842594%2C54.46001700833452%2C18.550592064857486%2C54.46113953783808&amp;layer=mapnik&amp;marker=54.46057827693473%2C18.549250960350037"
			/>

		
	</div>  
</section>

<!-- <section class="community-section mb-24 mt-24">
<a name="community"></a>

</section> -->




<style>
.social-coordinator-container {
  font-size: 2.5em;
  height: 60px;
  max-width: 360px;
}


.fb-mode {
  color: #ea4c89;
}

.ln-mode {
  color: #00A5E6;
}

.gh-mode {
  color: #4A148C;
}

	.boardgames-section {

	}

	.tools-section {

	}

	.faq-section {

	}

	.contact-section {

	}

	.community-section {

	}
</style>