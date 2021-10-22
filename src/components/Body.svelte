<script>
	export let quote = '',
		author = '',
		text = '';
</script>

<div>
	<h1>{quote}<span>{author}</span></h1>
	<p>{text}</p>
</div>

<style>
	div {
		text-align: center;
		display: flex;
		flex-direction: column;
		padding: 1em;
	}
	span {
		font-style: normal;
		font-size: 16px;
	}
	h1 {
		font-size: 16px;
		font-style: italic;
	}
	p {
		font-size: 13px;
	}
	@media screen and (max-width: 375px) {
		h1,
		span {
			font-size: 14px;
		}
		p {
			font-size: 11px;
		}
	}
</style>
