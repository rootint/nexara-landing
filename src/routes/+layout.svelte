<script>
	import './styles.css';
	import './fonts.css';
	import Header from './components/Header.svelte';
</script>

<div class="app">
	<Header></Header>
	<main>
		<slot />
	</main>
	<!-- <Footer /> -->
</div>
