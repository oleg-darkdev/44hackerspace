<script>
    import WhatWeDoCard from "./bio/WhatWeDoCard.svelte";
    import PaperYellow from '../layout/PaperYellowSetcionWrapper.svelte';
    import BioCard from '../components/bio/BioCard.svelte';


    const WhatWeDoInfo = [
        {
            heading: 'Druk 3d',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: false,
            img: '/about/3d.png',
            link: '/workshop#printer'
        },
        {
            heading: 'Wypożyczalnia gier planszowych',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: true,
            img: '/about/boardgames.png',
            link: '/library'
        },
        {
            heading: 'Wycinanie i grawerowanie laserowe',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: false,
            img: '/about/laser.png',
            link: '/workshop#laser'
        },
        {
            heading: 'Turnieje szachowe',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: true,
            img: '/about/chess.png',
            link: 'https://yellow-elephant.vercel.app/'
        },
    ];


    const DescriptionText = [
       
            {
                heading: 'Z Białorusi z miłością',
                description: 'Przestrzeń, stworzona przez uchodźcę politycznego z Białorusi, z myślą do wspólnej twórczości i technicznej edukacji.'
            },
            {
                heading: 'Edukacyjne gry planszowe',
                description: 'Popularyzacja edukacyjnych gier planszowych, projektowanie i wykonywanie własnych gier planszowych.'
            },
            {
                heading: 'Dostępność dla wszystkich',
                description: 'Bardzo zależy na tym, aby przestrzeń była przyjazna i otwarta dla jak najszerszej grupy odbiorców. Także dla uchodźców z krajów byłego Związku Radzieckiego.'
            },
            {
                heading: 'Otwarte warsztaty',
                description: 'Tematyka tradycyjnie pokrywa się z szeroko pojętym IT, programowaniem, Open Source, elektroniką oraz CNC, 3D.'
            }
        ] 
</script>

<div class="w-12/12 -mb-52 -mt-52 flex flex-row justify-center flex-wrap ">
<a name="mission"></a> 
<PaperYellow>
    {#each DescriptionText as text}
        <BioCard {text}/>
    {/each}
</PaperYellow>
</div>



<div  class="w-12/12 mt-52 flex flex-col pb-12 pt-12 justify-center flex-wrap" style="background-color: #f3e600;" >
    <a name="service"></a> 

    <h2 class="lg:text-7xl text-5xl text-center mb-2 text-dark font-impact">Dostępne dla gości</h2>
    <div class="flex flex-wrap w-full flex-row place-items-center">
    {#each WhatWeDoInfo as weDo}
        <WhatWeDoCard heading={weDo.heading} description={weDo.description} img={weDo.img} reverse={weDo.reverse} href={weDo.link}/>
    {/each}
    </div>
</div>