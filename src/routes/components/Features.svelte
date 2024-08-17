<script>
	import dataCollection from '$lib/assets/data.png';
	import cheapness from '$lib/assets/cheap.png';
	import easeOfUse from '$lib/assets/ease.svg';
	import apiImage from '$lib/assets/api.svg';
	import russianFlag from '$lib/assets/ru.png';
	import MainButton from './MainButton.svelte';
</script>

<section class="features" id="features">
	<h2>Мощные возможности, простые решения</h2>
	<h3>От сбора данных до развертывания - всё под Вашим контролем.</h3>
	<div class="bento-grid">
		<div class="grid-element data-card">
			<img src={dataCollection} alt="Графика показывает сбор данных с моделей." />
			<div class="text-block">
				<h4>Сбор данных</h4>
				<p class="h4-subtitle">Сохраняйте все промпты и запросы к Вашим LLM.</p>
			</div>
		</div>
		<div class="grid-element cheap-card">
			<img
				src={cheapness}
				alt="Графика показывает дешевизну использования Nexara, наши модели дешевле в 5 раз!"
			/>
			<div class="text-block">
				<h4>Дешевизна</h4>
				<p class="h4-subtitle">Экономьте на LLM без потери качества.</p>
			</div>
		</div>
		<div class="grid-element ease-card">
			<img
				src={easeOfUse}
				alt="Графика показывает простоту использования, модели можно обучать в два клика"
			/>
			<div class="text-block">
				<h4>Удобство</h4>
				<p class="h4-subtitle">Обучайте и развертывайте модели за пару кликов.</p>
			</div>
		</div>
		<div class="grid-element ru-card">
			<img src={russianFlag} width="76px" alt="Графика показывает флаг России" />
			<div class="text-block">
				<h4>Работает на русском</h4>
				<p class="h4-subtitle">Все модели оптимизированы под русский язык.</p>
			</div>
		</div>
		<div class="grid-element api-card">
			<img
				src={apiImage}
				alt="Графика показывает строки кода, показывающие, насколько просто интегрировать Nexara в свой продукт"
			/>
			<div class="text-block">
				<h4>Простой API</h4>
				<p class="h4-subtitle">С легкостью интегрируйте наши модели за пару строчек кода.</p>
			</div>
		</div>
		<div class="grid-element cta-card">
			<div class="text-container">
				<h4>Напишите нам</h4>
				<p class="h4-subtitle">А мы Вам назначим ознакомительную встречу.</p>
			</div>
			<MainButton theme="light"></MainButton>
		</div>
	</div>
</section>

<style>
	.features {
		display: flex;
		flex-direction: column;
	}
	.bento-grid {
		display: grid;
		gap: 32px;
		grid-template-columns: repeat(12, 1fr);
		grid-template-rows: auto;
		margin-bottom: 172px;
		margin-top: 64px;
	}

	.bento-grid img {
		max-width: 100%;
		max-height: 100%;
		object-fit: contain; /* or "cover" depending on your design needs */
	}

	.grid-element {
		padding: 32px;
		border-radius: 12px;
		background-color: var(--bg-2);
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		align-items: center;
	}

	.data-card {
		grid-column: span 7;
		grid-row: span 2;
	}

	.cheap-card {
		grid-column: span 5;
		grid-row: span 2;
	}

	.ease-card {
		grid-column: span 5;
		grid-row: span 2;
	}

	.ru-card {
		grid-column: span 4;
		grid-row: span 1;
	}

	.api-card {
		grid-column: span 3;
		grid-row: span 1;
	}

	.cta-card {
		grid-column: span 7;
		grid-row: span 1;
		background-color: #222;
		align-items: start;
		justify-content: space-between;
		display: flex;
		flex-direction: row;
	}
	.text-container {
		padding-right: 16px;
	}
	.text-container h4 {
		color: var(--bg);
		text-align: start;
	}
	.text-container p {
		color: #ccc;
		text-align: start;
	}

	@media (max-width: 1200px) {
		.bento-grid {
			display: grid;
			gap: 20px;
			grid-template-columns: repeat(12, 1fr);
			grid-template-rows: auto;
			margin-bottom: 96px;
			margin-top: 48px;
		}
		.ru-card {
			grid-column: span 7;
			grid-row: span 1;
		}
		.ru-card .text-block {
			margin-top: 16px;
		}

		.api-card {
			grid-column: span 7;
			grid-row: span 1;
		}

		.cta-card {
			grid-column: span 12;
			grid-row: span 1;
		}
		.grid-element {
			padding: 24px;
		}
	}

	@media (max-width: 960px) {
		.ease-card {
			grid-column: span 7;
			grid-row: span 2;
		}
		.ru-card {
			grid-column: span 5;
			grid-row: span 1;
		}
		.api-card {
			grid-column: span 5;
			grid-row: span 1;
		}
		.cta-card {
			background-color: #222;
			align-items: center;
			justify-content: center;
			display: flex;
			flex-direction: column;
		}
		.text-container {
			padding-right: 0px;
		}
		.text-container h4 {
			color: var(--bg);
			text-align: center;
		}
		.text-container p {
			color: #ccc;
			text-align: center;
			margin-bottom: 24px;
		}
	}

	@media (max-width: 800px) {
		.bento-grid {
			display: flex;
			flex-direction: column;
			margin-bottom: 72px;
			margin-top: 32px;
		}
		.ru-card .text-block {
			margin-top: 24px;
		}
		.api-card .text-block,
		.ease-card .text-block,
		.cheap-card .text-block {
			margin-top: 16px;
		}
	}
</style>
