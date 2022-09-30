<script>
	import Carousel from '../components/Carousel.svelte';
	import Workshops from '../components/Workshops.svelte';
	import Contact from '../components/Contact.svelte';
	import Bio from '../components/Bio.svelte'; 
	import YellowSetcionWrapper from '../layout/YellowSetcionWrapper.svelte';
	import BoardgamesList from '../components/BoardgamesList.svelte'
</script>

<Carousel />
<!-- workshops-section -->
<section class="bio-section mb-24 mt-24"> 
	<a name="bio"></a> 
	
	<Bio />
</section>

<section class="boardgames-section mb-24 mt-24" > 
	<a name="boardgames"></a> 
	<BoardgamesList />
</section>

<section class="workshops-section mb-24 mt-24">
	<a name="workshops"></a>
	<YellowSetcionWrapper>
		<Workshops />
	</YellowSetcionWrapper>
</section>

<section class="tools-section mb-24 mt-24">
<a name="tools"></a>
</section>

<section class="faq-section mb-24 mt-24">
<a name="faq"></a>

</section>


<section class="contact-section mb-24 mt-24">
<a name="contact"></a>
<div style="background-color: #f3e600;" class="workshops-section p-12 h-auto lg:w-12/12 px-8 sm:w-12/12  flex flex-row justify-center content-center ">
	<Contact />
</div>
</section>

<section class="community-section mb-24 mt-24">
<a name="community"></a>

</section>


<style>
	.workshops-section {
		/* padding: 50px 0;
		background-color: #f3e600; */
		/* width: 650px; */
		display: flex;
		/* padding: 50px; */
		justify-content: center;
		align-content: center;
		
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