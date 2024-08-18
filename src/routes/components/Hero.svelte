<script>
	import CompanySlider from './CompanySlider.svelte';
	import MainButton from './MainButton.svelte';
	import ProductRadar from './ProductRadar.svelte';
</script>

<section class="hero">
    <div class="animate-text">
        <ProductRadar></ProductRadar>
		<h1 class="title">Сократите расходы на LLM в 5 раз</h1>
		<p class="subtitle">
			Создавайте более быстрые и дешевые модели на основе своих данных. Без знаний ML.
		</p>
	</div>
	<div class="animate">
		<MainButton></MainButton>
	</div>
	<CompanySlider></CompanySlider>
</section>

<style>
	.hero {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin: 0 auto;
		height: 100vh;
		position: relative;
		min-height: -webkit-fill-available;
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

	@media (max-height: 720px) {
		.hero {
			height: 720px;
		}
	}

	@media (max-width: 900px) {
		.hero {
			height: 800px;
		}
		.subtitle {
			font-size: 20px;
			max-width: 560px;
			text-align: center;
			margin-bottom: 48px;
		}
	}
</style>
