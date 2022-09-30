<script>
    import WhatWeDoCard from "./bio/WhatWeDoCard.svelte";


    const WhatWeDoInfo = [
        {
            heading: 'Noteworthy technology acquisitions 2021',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: false,
            img: 'https://raw.githubusercontent.com/oleg-darkdev/44hackerspace/dev/static/about/3d.png'
        },
        {
            heading: 'Noteworthy technology acquisitions 2021',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: true,
            img: 'https://raw.githubusercontent.com/oleg-darkdev/44hackerspace/dev/static/about/boardgames.png'
        },
        {
            heading: 'Noteworthy technology acquisitions 2021',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: false,
            img: 'https://raw.githubusercontent.com/oleg-darkdev/44hackerspace/dev/static/about/laser.png'
        },
        {
            heading: 'Noteworthy technology acquisitions 2021',
            description: 'Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.',
            reverse: true,
            img: ''
        },
    ]
</script>

<div  class="w-12/12 mb-24 mt-24 flex flex-row space-between flex-wrap ">
{#each WhatWeDoInfo as weDo}
    <WhatWeDoCard heading={weDo.heading} description={weDo.description} position={weDo.position} img={weDo.img} reverse={weDo.reverse}/>
{/each}
</div>