<script>
	import Quote from "../src/lib/components/quotes.svelte";
	export let name;


</script>


<main>
	<h1>Hello {name}!</h1>
</main>
<div class="mx-auto flex max-w-2xl flex-col items-start justify-center">
	<section class="flex flex-col-reverse items-start sm:flex-row">
		<div class="container">
			<h3 class="mb-6 text-2xl font-bold tracking-tight md:text-4xl">
				Random Quotes
			</h3>
		</div>

		<div class="container">
			<div>
				<Quote />
			</div>
		</div>
	</section>
</div>


<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	.container {
		margin-left: 100px;
		margin-right: 100px;

	}

	h1 {
		color: rebeccapurple;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	h3 {
		font-weight: 400;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>