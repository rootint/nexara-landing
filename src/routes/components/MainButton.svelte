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
		background: linear-gradient(to right, #222 70%, #444);
		padding: 24px 36px;
		border-radius: 12px;
		border: none;
		cursor: pointer;
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
	}

	.light {
		background: linear-gradient(to right, #fff 70%, rgba(255, 255, 255, 0.5));
		color: #222;
	}
</style>
