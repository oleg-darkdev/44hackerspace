<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
	// import Footer from '../components/Footer.svelte';
</script>

<Header />

<slot />

<!-- <Footer /> -->

<style>
	:global(.social-hover:hover) {
	  background-color: #F3E600;
	}

	:global(.social-coordinator-container) {
    font-size: 2.5em;
    height: 60px;
    max-width: 360px;
  }
</style>