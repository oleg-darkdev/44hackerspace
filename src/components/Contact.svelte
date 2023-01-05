<script>
  import { Avatar, Dropdown, DropdownHeader, DropdownItem, DropdownDivider, Tooltip } from "flowbite-svelte";

  const hackerspacesList = [
    {
      link: 'https://hs3.pl/',
      local: 'Gdansk',
      logo: '/hackerspaces/hst.png'
    },
    {
      link: 'https://lodz.hackerspace.pl/',
      local: 'Łódź',
      logo: '/hackerspaces/lodz.svg'
    },
    {
      link: 'https://wiki.hswro.org/',
      local: 'Wrocław',
      logo: '/hackerspaces/wroclaw.png'
    },
    {
      link: 'https://hsp.sh/',
      local: 'Gdansk',
      logo: '/hackerspaces/hsp.png'
    },
    {
      link: 'https://hackerspace-krk.pl/',
      local: 'Kraków',
      logo: '/hackerspaces/krakow.svg'
    },
    {
      link: 'https://hackerspace.pl/',
      local: 'Warszawa',
      logo: '/hackerspaces/wawa.svg'
    },
    {
      link: 'https://www.facebook.com/cumy.stocznia',
      local: 'Gdansk',
      logo: '/hackerspaces/cumy.jpg'
    },
    {
      link: 'https://www.facebook.com/FabLabT/',
      local: 'Gdynia',
      logo: '/hackerspaces/fablab.jpg'
    }
  ];
</script>

<div class="mb-6 w-full flex justify-center flex-col  bg-dark p-6 rounded-xl max-w-2xl">
<!-- Inne hackerspacy -->
	<h2
		class="text-4xl font-impact tracking-tight leading-none text-white md:text-3xl lg:text-3xl text-center"
	>
		Inne hackerspacy
	</h2>
  <p class="pr-4 pl-4 mb-2 font-normal text-white text-center leading-tight">
    Hackerspace jest ideą ogólnoświatową. W wielu miastach w Polsce i na świecie możesz spotkać się z przestrzeniami o tej samej lub podobnej nazwie, takie jak Makerspace, Hacklab czy nawet FabLab. Każda organizacja jest inna i oferuje inny zestaw doświadczeń.
  </p>

  <div class="flex flex-row justify-center flex-wrap">
  {#each hackerspacesList as hackerspace}
      
          <a 
              class="partners-logos rounded-lg m-1 hs-logos"
              style="background-image: url({hackerspace.logo});"
              href="{hackerspace.link}"
          />
          <!-- <h4 class="text-center"><a href={org.link} target="_blank">{org.title}</a></h4> -->
  {/each}
  </div>
</div>






<style>
  .hs-logos {
    background-color: #fff; background-repeat: no-repeat; background-position: center;  background-size:  contain; width: 200px; height: 100px;
  }
  .hs-logos:hover {
    background-color: #F3E600;
  }
</style>