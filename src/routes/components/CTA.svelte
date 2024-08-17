<script>
	import MainButton from './MainButton.svelte';
</script>

<section class="cta">
	<div class="text-container">
		<h2>Давайте познакомимся!</h2>
		<p>Оставьте нам свои контакты и мы свяжемся с Вами.</p>
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

	@media (max-width: 1200px) {
		.cta {
			margin-top: 96px;
			margin-bottom: 96px;
        }
	}

	@media (max-width: 1000px) {
		.cta {
			flex-direction: column;
			align-items: center;
			justify-content: center;
			margin-top: 72px;
			margin-bottom: 72px;
		}
		h2 {
			text-align: center;
		}

		p {
			text-align: center;
			font-size: 16px;
			margin-bottom: 24px;
		}

		.text-container {
			display: flex;
			flex-direction: column;
			align-items: center;
		}
	}
</style>
