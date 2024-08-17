<script>
	import { ArrowUpRight } from 'lucide-svelte';

	export var theme = 'dark';
</script>

{#if theme === 'dark'}
	<a
		href="https://docs.google.com/forms/d/e/1FAIpQLSd6SasqzSD3w_gI49MOV6lrMKel3Sbxhhoee8hopLFDQJJhUg/viewform"
	>
		<button class="cta-btn">
			<div class="row">
				<p>Оставить Заявку</p>
				<div class="icon">
					<ArrowUpRight color="#fff"></ArrowUpRight>
				</div>
			</div>
		</button>
	</a>
{:else if theme === 'light'}
	<a
		href="https://docs.google.com/forms/d/e/1FAIpQLSd6SasqzSD3w_gI49MOV6lrMKel3Sbxhhoee8hopLFDQJJhUg/viewform"
	>
		<button class="cta-btn light">
			<div class="row">
				<p class="light">Оставить Заявку</p>
				<div class="icon">
					<ArrowUpRight color="#222"></ArrowUpRight>
				</div>
			</div>
		</button>
	</a>
{/if}

<style>
	.cta-btn {
		background-image: linear-gradient(to right, #222 0%, #555 50%, #222 100%);
		background-size: 200% auto;
		padding: 24px 36px;
		border-radius: 12px;
		border: none;
		cursor: pointer;
		min-width: 274px;
		transition: background-position 0.5s ease-out;
	}
	.cta-btn:hover {
		animation: gradient-shift 2s linear infinite;
	}
	.row {
		display: flex;
	}
	.icon {
		margin-top: 2px;
	}
	p {
		margin-right: 12px;
		color: #fff;
		font-weight: 450;
		font-size: 20px;
		background-color: none;
	}

	.light {
		background-image: linear-gradient(to right, #fff 0%, #ddd 50%, #fff 100%);
		background-size: 200% auto;
	}
	.light p {
		color: #222;
		background-color: none;
		background-image: none;
	}

	@keyframes gradient-shift {
		0% {
			background-position: 0% center;
		}
		100% {
			background-position: -200% center;
		}
	}
</style>
