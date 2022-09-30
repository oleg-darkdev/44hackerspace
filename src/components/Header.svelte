<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { DarkMode } from 'flowbite-svelte';
  let darkmodebtn =
		'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-lg p-2.5 fixed right-4 top-2 z-50';

</script>


<Navbar let:hidden let:toggle>
  <NavBrand href="/">
    <img
      src="https://flowbite.com/docs/images/logo.svg"
      class="mr-3 h-6 sm:h-9"
      alt="Flowbite Logo"
    />
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
      Flowbite
    </span>
  </NavBrand>
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="#bio">Bio</NavLi>
    <NavLi href="#tools">Tools</NavLi>
    <NavLi href="#boardgames">Boardgames</NavLi>
    <NavLi href="#workshops">Workshops</NavLi>
    <NavLi href="#faq">Faq</NavLi>
    <NavLi href="#contact">Contact</NavLi>
    <NavLi href="#community">Community</NavLi>
    <!-- <DarkMode  /> -->
  </NavUl>
</Navbar>