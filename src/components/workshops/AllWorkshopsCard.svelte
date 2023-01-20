<script>
    let showFullWorkshopsList = false;

    export let workshopsCounter;
</script>


<div style="" class="p-4 sm:p-6 flex items-center bg-dark border border-gray-200 shadow-md text-gray-500 rounded-lg flex flex-col max-w-2xl">
      <dir class=" flex items-center flex-row w-full">
         <span class="max:w-7/12 pt-8 mr-2 text-end text-3xl text-current font-impact">
          W ciągu historii naszeо aktywności istnienia zorganizowaliśmy
         </span>
         <p class=" flex flex-col items-start ">
            <span class=" text-7xl -mb-4 text-center text-white font-impact">
              {workshopsCounter}
          </span>      
          <span class="text-3xl text-center text-current font-impact">
              warsztatów
          </span>     
         </p>          
      </dir>
      <a name="history">
      </a>
                  
      {#if showFullWorkshopsList}
        <slot></slot>
      {/if}

        <button type="button" on:click={() => showFullWorkshopsList = !showFullWorkshopsList} class="lg:w-6/12 md:w-6/12 w-6/12 text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-6 py-3.5 text-base text-dark bg-current hover:bg-white focus:ring-white rounded-lg">
             {showFullWorkshopsList ? 'Schowaj': 'Czytaj'} całą listę
        </button>
  </div>