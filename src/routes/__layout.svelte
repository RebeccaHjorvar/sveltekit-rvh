<script>
	import Hero from '../components/Hero.svelte';
	import Nav from '../components/Nav.svelte';
</script>

<div class="wrapper">
	<div class="nav">
		<Hero />
		<Nav />
	</div>
	<slot />
</div>

<style lang="postcss">
	.wrapper {
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.nav {
		display: flex;
		flex-direction: column;
		flex-wrap: wrap;
        margin: 5% auto;
	}
	:global(body) {
		background-color: #2a2b2a;
		color: #99df3b;
		font-family: sans-serif;
	}
	@media screen and (max-width: 475px) {
		:global(body) {
			font-size: 13px;
		}
	}
	@media screen and (min-width: 1440px) {
		.nav {
			flex-direction: row;
            align-items: center;
            flex-wrap: nowrap;
		}
	}
</style>
