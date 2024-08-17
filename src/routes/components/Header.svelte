<script>
</script>

<header>
	<nav>
		<div class="top-row">
			<img src="favicon.png" height="32" width="32" alt="logo" />
			<div style="width: 8px" />
			<p class="logo">Nexara</p>
		</div>
		<div class="top-row">
			<div class="hide-on-mobile">
				<a href="#features"><p>Особенности</p></a>
				<div style="width: 4rem" />
				<a href="#pricing"><p>Тарифы</p></a>
			</div>
		</div>
	</nav>
</header>

<style>
	.logo {
		font-weight: 500;
	}
	a {
		text-decoration: none;
	}
	.hide-on-mobile {
		display: flex;
		align-items: center;
	}
	@media (max-width: 768px) {
		.hide-on-mobile {
			display: none;
		}
	}
	nav {
		color: #fff;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin: 0 0;
		margin-top: 24px;
	}

	@media (max-width: 768px) {
		nav {
			color: #fff;
			display: flex;
			justify-content: space-between;
			align-items: center;
			margin: 0 0;
			padding-top: 0px;
		}
	}

	.top-row {
		display: flex;
		align-items: center;
	}

	p {
		font-weight: 400;
		font-size: 1rem;
	}
</style>
