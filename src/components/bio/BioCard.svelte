<script>
  import { Card } from "flowbite-svelte";


  export let text;
</script>

<Card  class="m-1">
  <h5 class="mb-2  text-2xl font-impact text-gray-700 ">{text.heading}</h5>
  <p class="font-normal text-gray-700 leading-tight">
    {text.description}
  </p>
</Card>