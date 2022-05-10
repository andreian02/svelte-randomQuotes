<script>
	import data from '../../assets/quotes.json';

	import { fade } from 'svelte/transition';
	let options = { duration: 400 };

	export let quotes = data;
	let quote = getRandomQuote(quotes);

	function getRandomQuote(quotes) {
		return quotes[Math.floor(Math.random() * quotes.length)];
	}

	function updateQuote() {
		quote = getRandomQuote(quotes);
	}
</script>

<div class="box">
	<blockquote>
		{#key quote}
			<div in:fade={options}>
				<p class="quote content">{quote.quote}</p>
				<footer> {quote.author}</footer>
			</div>
		{/key}
	</blockquote>
</div>

<button on:click={updateQuote} type="submit">
	<span class="icon"><i class="fas fa-redo" /></span>
	<span>Generate Quote</span>
</button>

<style>
    span {
        color: rebeccapurple;
    }

	footer {
		font-weight: 500;
		margin-left: 3rem;
	}
	footer::before {
		content: '\2014 ';
	}
	blockquote {
		margin-bottom: 2rem;
	}
</style>
