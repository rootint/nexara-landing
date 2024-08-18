<script>
	import './styles.css';
	import './fonts.css';
	import Header from './components/Header.svelte';
	import rect1 from '$lib/assets/rect1.svg';
	import rect2 from '$lib/assets/rect2.svg';
    import rect3 from '$lib/assets/rect3.svg';
</script>

<div class="background">
	<img src={rect1} id="rect1" />
	<img src={rect2} id="rect2" />
    <img src={rect3} id="rect3" />
</div>
<div class="app">
	<Header></Header>
	<main>
		<slot />
	</main>
	<!-- <Footer /> -->
</div>

<style>
	.background {
		position: absolute;
        margin: 0 auto 0;
		width: 100%;
		height: 100vh;
		overflow: hidden;
	}
	#rect1 {
		position: absolute;
		left: 0px;
	}
	#rect2 {
		position: absolute;
		right: 0px;
	}
    #rect3 {
		position: absolute;
		right: 0px;
        bottom: 0px;
	}
</style>
