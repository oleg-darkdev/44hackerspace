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
		background-color: #f3e600;
	}

	:global(.social-coordinator-container) {
		font-size: 2.5em;
		height: 60px;
		max-width: 360px;
	}

	:global(.font-impact) {
		font-family: 'Impact';
		line-height: 1.2;
	}

	@font-face {
		font-family: 'Impact';
		font-style: normal;
		font-weight: 500;

		src: local(''), /* Super Modern Browsers */ url('/fonts/impact.woff') format('woff'),
			/* Modern Browsers */ url('/fonts/impact.ttf') format('truetype'),
			/* Safari, Android, iOS */ url('/fonts/impact.svg') format('svg'); /* Legacy iOS */
	}
</style>
