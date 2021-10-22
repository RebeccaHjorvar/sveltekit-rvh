<script>
	import { educationIcon, experienceIcon } from '../svg-handler';
</script>

<div class="cta">
	<a href="/education" id="educationLink" class="icon">{@html educationIcon}</a>
	<a href="/experience" id="experieceLink" class="icon">{@html experienceIcon}</a>
	<a href="/future" id="futureLink" class="icon">{@html educationIcon}</a>
</div>

<style lang="postcss">
	.cta {
		display: flex;
		flex-direction: row;
	}
	.icon {
		width: 50px;
		height: 50px;
		fill: #99df3b;
	}
	a {
		padding: 1em;
		margin: 0em;
	}
	a:hover {
		cursor: pointer;
		background-color: #99df3b;
		fill: #2a2b2a;
		border-radius: 50%;
		transform: rotate(-10deg);
	}
	@media screen and (min-width: 1440px) {
		.cta {
			flex-direction: column;
			align-items: center;
			justify-items: flex-end;
			flex-wrap: nowrap;
			margin-left: 10%;
		}
	}
</style>
