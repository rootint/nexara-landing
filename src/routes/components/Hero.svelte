<script>
	import MainButton from './MainButton.svelte';
</script>

<section class="hero">
	<div class="animate-text">
		<h1 class="title">Сократите расходы на LLM в 5 раз</h1>
		<p class="subtitle">
			Создавайте более быстрые и дешевые модели на основе своих данных. Без знаний ML.
		</p>
	</div>
	<div class="animate">
		<MainButton></MainButton>
	</div>
</section>

<style>
	.hero {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 95vh;
	}
	.title {
		text-align: center;
		max-width: 768px;
		margin-bottom: 40px;
		background: linear-gradient(to bottom, #222 50%, #666 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
	}

	.animate-text {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		animation: slideUp 0.7s ease;
	}

	.animate {
		animation: fadeIn 0.7s ease;
	}

	.subtitle {
		font-size: 24px;
		max-width: 560px;
		text-align: center;
		margin-bottom: 64px;
	}
</style>
