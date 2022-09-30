<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
	import { DarkMode } from "flowbite-svelte";

</script>
<Header />

<slot />


<!-- <DarkMode /> -->
<Footer />