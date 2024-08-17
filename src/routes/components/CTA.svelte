<script>
	import MainButton from './MainButton.svelte';
</script>

<section class="cta">
	<div class="text-container">
		<h2>Давайте познакомимся!</h2>
		<p>Оставьте нам свои контакты и мы свяжемся с вами.</p>
	</div>
	<MainButton theme="light"></MainButton>
</section>

<style>
	.cta {
		display: flex;
		justify-content: space-between;
		background-color: var(--text);
		border-radius: 12px;
		padding: 48px;
        margin-top: 172px;
        margin-bottom: 172px;
	}

	h2 {
		color: var(--bg);
	}

	p {
		color: var(--bg);
        font-size: 20px;
        font-weight: 400;
	}
    .text-container {
        display: flex;
        flex-direction: column;
        align-items: start;
    }
</style>
