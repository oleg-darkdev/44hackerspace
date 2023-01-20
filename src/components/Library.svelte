<script>
    import boardgamesList from '../data/boardgamesList';        
</script>

<div class="w-12/12 -mb-52 -mt-52 flex flex-row justify-center flex-wrap ">
<div style="background-color: #f3e600;" class="workshops-section rounded-2xl mb-12 mt-12 lg:w-7/12 px-8 sm:w-8/12 h-auto p-10 flex flex-col flex-wrap justify-center content-center ">
        <h2 class="lg:text-7xl text-5xl  text-center mb-2 text-dark font-impact">Wypożyczalnia gier planszowych</h2>

        <div class="flex flex-row w-full flex-wrap justify-center ">
        {#each boardgamesList as boardgame}
            <div class="m-1 bg-white dark:bg-gray-800 text-gray-500 dark:text-gray-400 rounded-lg border border-gray-200 dark:border-gray-700 shadow-md flex max-w-sm flex-col">
                <img style="" class="rounded-t-lg" src="{boardgame.img}" alt="{boardgame.title}"> 
                <div class="p-4 sm:p-6">
                    <h5 class="mb-2 text-2xl font-impact text-gray-700">
                        {boardgame.title}
                    </h5> 
                    {#each boardgame.description as text}
                        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
                            {text}
                        </p> 
                    {/each}
                       <a href='{boardgame.link}' class="w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-dark hover:bg-dark focus:ring-blue-300 rounded-lg">
                            Czytaj więcej
                        </a>
                </div>
            </div>

        {/each}
    </div>
</div>
</div>
        

