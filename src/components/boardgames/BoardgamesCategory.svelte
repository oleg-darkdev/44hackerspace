<script>
  import { Accordion, AccordionItem } from 'flowbite-svelte';
import BoardgamesItem from './BoardGamesItem.svelte';
import { Img } from 'flowbite-svelte';

//   export let categoryList;
</script>


<Accordion
  activeClasses="bg-blue-100 dark:bg-gray-800 text-blue-600 dark:text-white focus:ring-4 focus:ring-blue-200 dark:focus:ring-blue-800"
  inactiveClasses="text-gray-500 dark:text-gray-400 hover:bg-blue-100 dark:hover:bg-gray-800">
  <AccordionItem>
    <h2 slot="header">Header 2-1</h2>
    <div slot="body">
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
    </div>
  </AccordionItem>
  <AccordionItem>
    <h2 slot="header">Header 2-2</h2>
    <div slot="body">
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
    </div>
  </AccordionItem>
</Accordion>