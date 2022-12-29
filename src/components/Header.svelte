<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>


<Navbar let:hidden let:toggle>
  <NavBrand href="/">
    <img loading="lazy" src="/logo.svg" class="rounded-lg h-20 " alt="ITingo Logo"/>
    <!-- <span class="self-center whitespace-nowrap lg:text-5xl md:text-4xl  text-3xl   text-lightYellow text-stantley">
      ITingo
    </span> -->
  </NavBrand>

  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="#contact">Kontakt</NavLi>
    <NavLi href="#mission">Nasza misja</NavLi>
    <NavLi href="#service">Dostępne dla gości</NavLi>
    <NavLi href="#workshops">Warsztaty</NavLi>
    <NavLi href="/library">Wypożyczalnia gier planszowych</NavLi>
    <!-- <NavLi href="#faq">Faq</NavLi> -->
    
    <!-- <NavLi href="#community">Community</NavLi> -->
  </NavUl>
</Navbar>