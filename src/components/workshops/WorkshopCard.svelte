<script>
	export let workshopData;
</script>


<div
	class="w-11/12  pr-2 pl-2 pb-1 m-2 bg-current border border-gray-200 shadow-md text-gray-500 rounded-lg flex flex-col max-w-2xl"
>
	<img class="rounded-t-lg" style="width: 760px; " src={workshopData.img} alt="" />
	<div class=" sm:p-6">
		<h5 class="mb-2 text-2xl font-impact text-dark worhshop">
			{workshopData.title}
		</h5>

		{#each workshopData.description as description}
			<p style="" class="pl-2 mb-1 font-normal  text-dark leading-tight">
				{description}
			</p>
		{/each}

		{#if workshopData.showFullInfo}
			<div class="mb-2 bg-current text-gray-500 rounded-lg flex w-full flex-col p-2 sm:p-4">
				<div class="flex justify-between items-center">
					<h5 class="text-xl mb-2 font-impact text-dark worhshop">Niedawne warsztaty</h5>
				</div>
				<slot />
			</div>

			<div class="flex flex-col p-1 m-1 items-center w-full">
				<h5 class="text-xl mb-2 font-impact text-dark ">Partnerzy warsztatów</h5>

				<div class="flex flex-row w-full justify-center flex-wrap">
					{#each workshopData.partners as partner}
						<div
							class="partners-logos rounded-lg m-1"
							style="background-image: url({partner.logo}); width: 180px; height: 80px;"
						/>
						<!-- <h4 class="text-center"><a href={org.link} target="_blank">{org.title}</a></h4> -->
					{/each}
				</div>
			</div>
		{/if}

		<button
			type="button"
			on:click={() => (workshopData.showFullInfo = !workshopData.showFullInfo)}
			class="mt-10 w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-6 py-3.5 text-base text-white bg-dark hover:bg-dark focus:ring-white rounded-lg"
		>
			Czytaj {workshopData.showFullInfo ? 'mniej' : 'więcej'}
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
