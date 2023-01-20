<script>
  import Carousel from '../components/Carousel.svelte';
  import WorkshopCard from '../components/WorkshopCard.svelte';
  import Contact from '../components/Contact.svelte';
  import Bio from '../components/Bio.svelte';
  import socialCordinatorLinks from '../data/socialCordinatorLinks';
  import socialHackerspaceLinks from '../data/socialHackerspaceLinks';
  import workshopsList from '../data/workshopsList';
  import ListWorkshops from '../components/workshops/ListWorkshops.svelte';
  import AllWorkshopsList from '../components/AllWorkshopsList.svelte';
	// import AllWorkshops from '../components/AllWorkshopsList.svelte';



  $: workshopsCounter=workshopsList[0].schedule.length + workshopsList[1].schedule.length + workshopsList[2].schedule.length + workshopsList[3].schedule.length;
</script>


<Carousel bg='main-route'/>
<section class=""> 
  <Bio />
</section>

<section class="flex  bg-white pt-12 justify-center flex-col items-center pb-14">
  <a name="workshops">
  </a>
  <h2 class="lg:text-7xl text-5xl text-center text-dark font-impact">
    Lista warsztatów
  </h2>
  <AllWorkshopsList {workshopsCounter}>
    {#each workshopsList as workshopData}
      <div class="mb-4 bg-current text-gray-500 rounded-lg flex w-full flex-col p-2 sm:p-4">
            <h5 class="text-xl mb-2 font-impact text-dark dark:text-white">
                Wcześniejsze warsztaty: {workshopData.title}
            </h5> 
            <ListWorkshops workshopsHistory={workshopData.schedule} />     
      </div>
    {/each}
  </AllWorkshopsList>

  {#each workshopsList as workshopData}
    <WorkshopCard {workshopData}>
      <ListWorkshops workshopsHistory={workshopData.schedule} />
    </WorkshopCard>
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
  <a name="contact">
  </a>
  <h2
      class="mb-4 text-4xl font-impact tracking-tight leading-none text-white md:text-5xl lg:text-6xl text-center"
      >
    Skontaktuj się z nami
  </h2>
  <div
       style="max-width: 100%;"
       class="mb-4 max-w-sm bg-current flex flex-col items-center shadow-md rounded-lg border border-current  text-gray-500 p-6"
       >
    <div class="m-4 lg:w-6/12 md:w-8/12 w-12/12 flex flex-wrap justify-center flex-row bg-dark p-6 rounded-3xl">
      <h5 class="mb-2 text-2xl font-impacttracking-tight  text-white text-center">
        44hackerspace@gmail.com
      </h5>
      <h5 class="mb-2 text-2xl font-impacttracking-tight  text-white text-center">
        Mazowiecka 26, 81-862 Sopot, Poland
      </h5>
        <div class="w-full  flex flex-wrap justify-center content-center flex-row bg-dark mb-6 rounded-xl">
          <a href={socialHackerspaceLinks.facebook.link}>
            <img src="social/facebook.svg" class="w-20 h-20 rounded social-hover" alt="">

          </a>
          <a href={socialHackerspaceLinks.github.link}>
            <img src="social/github.svg" class="w-20 h-20 rounded social-hover" alt="">

          </a>
          <a href={socialHackerspaceLinks.linkedin.link}>
            <img src="social/linkedin.svg" class="w-20 h-20 rounded social-hover" alt="">

          </a>
          <a href={socialHackerspaceLinks.telegram.link}>
          <img src="social/telegram.svg" class="w-20 h-20 rounded social-hover" alt="">

          </a>
          <a href={socialHackerspaceLinks.patronite.link}>
            <img src="social/patronite.svg" class="w-20 h-20 rounded social-hover" alt="">
          </a>

        </div>

      <div  class="border border-white  flex max-w-sm flex-col m-2  dark:bg-gray-800 shadow-md text-gray-500 dark:text-gray-400 rounded-lg  dark:border-gray-700">
        <img loading="lazy" class="rounded-t-lg" src="/coordinator.png" alt=""> 
        <div class="p-1 rounded bg-lightYellow">
          <h5 class="mb-1 text-4xl font-impact   text-center tracking-tight text-white">
            Koordynator projektu
          </h5> 
          <p class="mb-3 font-impact text-5xl text-center text-white">
            Oleg Medvedev
          </p>
          <div class="w-full max-w-2xl flex flex-wrap justify-center content-center flex-row p-6 rounded-xl">
            <a href="{socialCordinatorLinks.facebook}">
              <img src="social/facebook.svg" class="w-20 h-20 rounded social-hover" alt="">
            </a>
            <a href="{socialCordinatorLinks.github}">
              <img src="social/github.svg" class="w-20 h-20 rounded social-hover" alt="">
            </a>
            <a href="{socialCordinatorLinks.linkedin}">
              <img src="social/linkedin.svg" class="w-20 h-20 rounded social-hover" alt="">
            </a>
            <a href="{socialCordinatorLinks.telegram}">
              <img src="social/telegram.svg" class="w-20 h-20 rounded social-hover" alt="">
            </a>
          </div>
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

</style>
