<script>


export let workshop;
</script>



<div style="" class="bg-current m-4 border border-gray-200 shadow-md text-gray-500 rounded-lg flex flex-col max-w-2xl">
        <img class="rounded-t-lg" style="width: 760px; " src={workshop.img} alt=""> 
    <div class="p-4 sm:p-6">
        {#if workshop.showFullInfo}
        <h5 class="mb-2 text-2xl font-impact text-dark dark:text-white">
            {workshop.title}
        </h5> 
        
            {#each workshop.description as description}
                <p style="" class="mb-1 font-normal  text-dark leading-tight">
                    {description}
                </p>
            {/each}


            <div class="mb-2 bg-current text-gray-500 rounded-lg flex w-full flex-col p-2 sm:p-4">
            <div class="flex justify-between items-center">
                <h5 class="text-xl mb-4 font-impact text-dark dark:text-white">
                    Niedawne warsztaty
                </h5> 
                <!-- <a href="/" class="text-sm font-medium text-blue-600 hover:underline dark:text-blue-500">View all
                </a> -->
            </div> 
            <ul class="bg-white w-full text-gray-500 rounded-lg border border-gray-200 divide-y divide-gray-200 border-0 ">
                {#each workshop.harmonogram as event}
                <li class="py-2 px-4 w-full text-sm font-medium first:rounded-t-lg last:rounded-b-lg">
                <div class="flex items-center space-x-4">
                    <!-- <img alt="Neil Sims" src="/images/profile-picture-1.webp" class="rounded-full w-10 h-10 bg-gray-100 dark:bg-gray-600 text-gray-600 dark:text-gray-300 flex-shrink-0">  -->
                    <div class="flex-1 min-w-0">
                    <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
                        {event.title}
                    </p> 
                    <p class="text-sm text-gray-500 truncate dark:text-gray-400">Mazowiecka 26, Sopot
                    </p>
                    </div> 
                    <div class="inline-flex items-center text-base font-semibold text-gray-900 dark:text-white">
                        {event.date}
                    </div>
                </div>
                </li>
                {/each}
            </ul>
            </div>

<div class="flex flex-col p-1 m-1 items-center ">
                <h5 class="text-xl mb-4 font-impact text-gray-700 text-dark dark:text-white">
                    Partnerzy warsztatów
                </h5> 

                <div class="flex flex-row flex-wrap pr-10 pl-10">
                    {#each workshop.partners as partner}
                        
                            <div
                                class="partners-logos rounded-lg m-1"
                                style="background-image: url({partner.logo}); width: 220px; height: 110px;"
                            />
                            <!-- <h4 class="text-center"><a href={org.link} target="_blank">{org.title}</a></h4> -->
                    {/each}
                </div>
            </div>
        {/if}

        <button type="button" on:click={() => workshop.showFullInfo = !workshop.showFullInfo} class="w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-6 py-3.5 text-base text-white bg-dark hover:bg-dark focus:ring-white rounded-lg">
            Czytaj {workshop.showFullInfo ? 'mniej': 'więcej'}
        </button>
    </div>
</div>



<style>
    .partners-logos {
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
	}
</style>