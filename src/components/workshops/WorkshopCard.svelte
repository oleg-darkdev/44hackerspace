<script>
  import { Card, Button, Toggle } from "flowbite-svelte";

  export let text, heading, btnLink;
</script>


<div class="p-2 justify-start w-12/12 flex">
  <Card  img="https://wallsdesk.com/wp-content/uploads/2017/01/Tel-Aviv-Photos.jpg" href={btnLink} horizontal reverse={false}>
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{heading}</h5>
    <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
      {text}
    </p>
    <!-- <div class="flex mt-4  lg:mt-6"> -->
        <Button color="light" class="dark:text-white" href={btnLink}>More</Button>
      <!-- </div> -->
  </Card>
</div>