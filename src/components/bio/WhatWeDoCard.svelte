<script>
  import { Card, Button} from "flowbite-svelte";

  export let heading, description, reverse, img, href;
</script>

<div class="md:w-3/12 ">
  <Card class="m-2 " img={img} reverse={reverse}>
    <h5 class="mb-1 text-2xl font-impact text-gray-700">{heading}</h5>
    <p class="mb-2 font-normal text-gray-700 dark:text-gray-400 leading-tight">
      {description}
    </p>
      <!-- <button type="button" on:click={() => showFullInfo = !showFullInfo} class="w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-6 py-3.5 text-base text-white bg-dark hover:bg-dark focus:ring-white rounded-lg">
          Czytaj {showFullInfo ? 'mniej': 'więcej'}
      </button> -->
      <a href='{href}' class="w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-dark hover:bg-dark focus:ring-blue-300 rounded-lg">
        Czytaj więcej
      </a>
  </Card>
</div>