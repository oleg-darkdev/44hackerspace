<script>
    export let workshopsHistory;
</script>

<ul class="bg-white  p-2 py-2 px-4       text-gray-500 rounded-lg border border-gray-200 divide-y divide-gray-200 border-0 ">
    {#each workshopsHistory as worhshop}
    <li class="text-gray-900 p-1 text-sm font-medium first:rounded-t-lg last:rounded-b-lg hover:text-current  hover:bg-dark">
    <div class="flex items-center space-x-4 ">
        <div class="flex-1 min-w-0 ">
            <p class="text-sm font-bold  truncate dark:text-white">
                {worhshop.title}
            </p> 
            <p class="text-sm  truncate ">Mazowiecka 26, Sopot
            </p>
        </div> 
        <div class="inline-flex items-center text-base font-semibold  ">
            {worhshop.date}
        </div>
            <a href="{worhshop.linkFb}" target="_blank" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex hover:bg-current items-center justify-center px-5 py-2.5 text-sm text-white bg-dark  focus:ring-yellow-300  rounded-lg !p-2">
                <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 15 22" xmlns="http://www.w3.org/2000/svg">
                    <path  fill-rule="evenodd"   d="M3,21.2c1.6,0,3.2,0,4.5,0v-9h3.8l0.8-4.5H7.6V4.5h4.6V0H7.6C5.1,0,3,2,3,4.5c0,0,0,0,0,0v3.1H0v4.5h3V21.2z"/>
                </svg>
            </a>
    </div>
    </li>
    {/each}
</ul>