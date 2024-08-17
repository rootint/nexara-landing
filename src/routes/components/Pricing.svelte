<script>
	import { Check } from 'lucide-svelte';
	import line from '$lib/assets/line.svg';
</script>

<section class="pricing" id="pricing">
	<h2>Тарифы</h2>
	<h3>Выберите план, подходящий вашему бизнесу.</h3>
	<div class="cards">
		<div class="card">
			<h4>Гибкий</h4>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Платите за то, что используете</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Автоматическое масштабирование</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">До 10 моделей</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">До 10 датасетов</p>
			</div>
			<div style="padding-bottom: 16px"></div>
			<img src={line} alt="Просто линия" />
            <div style="padding-bottom: 16px"></div>
			<p class="small-text">От 100₽ за миллион токенов за инференс и от 50₽ за обучение моделей.</p>
		</div>
		<div class="card">
			<h4>Кастомный</h4>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">То же самое, что и в Гибком тарифе</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Настройка на ваших серверах</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Приоритетная поддержка</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Увеличенное количество моделей</p>
			</div>
			<div class="option-container">
				<Check color="#222" size="20" />
				<p class="option-text">Увеличенное количество датасетов</p>
			</div>
		</div>
	</div>
</section>

<style>
	.cards {
		display: flex;
		justify-content: center;
		gap: 32px;
		margin-top: 64px;
	}
	.card {
		width: 440px;
		display: flex;
		flex-direction: column;
		align-items: start;
		background-color: var(--bg-2);
		border-radius: 12px;
		padding: 32px;
	}
	h4 {
		margin-bottom: 32px;
	}
	.option-container {
		display: flex;
		margin-bottom: 16px;
		align-items: start;
	}

	.option-text {
		margin-left: 8px;
	}
    .small-text {
        color: var(--text-2);
    }
</style>
